
# Actividades Examen

## Act 1

```
funcion void decimalBinario (int decimal) {
	while (decimal != 0) {
		print ( decimal % 2)
		decimal /= 2
	}
}
```

## Act 2
```
funcion void binarioDecimal ( long binario){
	double decimal = 0
	for (int i = 0; decimal != 0; i++) {
	int digit = (num) binario % 10
	decimal += digit * 2^i;
	binario /= 10
	}
	print (decimal)
}
```

## Act 3
```
funcion boolean esParell (int num){
	if (num%2 == 0){
		return (true)
	}else{
		return (-false)
	}
}
```

## Act 4
```
funcion void primersNombresParells(int num) {
	for (int i = 0; i <= num; i++) {
		if (esParell(i)) {
			print(i);
		}
	}
}
```

## Act 5
```
funcion int menu() {
	print(“Elije una de los siguientes opciones:”);
	print(“1. Decimal a binario”);
	print(“2. Binario a decimal”);
	print(“3. Es par?”);
	print(“4. Calcular pares de 0 hasta a n”);
	print(“0. Exit”);

	return = input();
}
```

## Act 6
```
main() {
	int opcion = menu();
	while (opcion != 0) {
		if (opcion == 1){
			print(“Introduce un numero decimal:”);
			int decimal = input();
			decimalBinari(decimal);
		} else if (opcion ==2){
			print(“Introduce un numero binario:”);
			long binario = input();
			binariDecimal(binario);
		} else if (opcion == 3){
			print(“Introduce un numero:”);
			int num = input();
			print(esParell(num));
		} else if (opcion == 4){
			print(“Introduce un numero maximo:”);
			int num = input();
			primersNombresParells(num);
		} else {
			print(“No has introducido un numero VALIDO”);
		}
	
		opcio = menu();
	}
}
```

## Act 7
a)
```
funcion double volumCilindre(double radi, double longitud) {
	return pi * radi^2 * longitud;
}
```

b)
```
funcion double volumPrismaRectangular(double c1, double c2, double c3) {
	return c1 * c2 * c3;
}
```

## Act 8
```
main() {
	println(“Que tenemos que transporta? 1. Liquidos 2. Solidos”);
	int opcion = input();
	while(opcion != 1 || opcion != 2) {
		print(“No és una opcion valido”);
		print(“Que tenemos que transporta? 1. Liquidos 2. Solidos”);
		opcion = input();
	}

	double volum = 0;
	if (opcion == 1) {
		print(“Dime el radio”);
		double radi = input();
		print(“Dime la longitud”);
		double llarg = input();
		volum = volumCilindre(radi, llarg);
	} else if (opcion == 2) {
		print(“Dime un costado”);
		double c1 = input();
		print(“Dime otro”);
		double c2 = input();
		print(“Dime la ultima medida”);
		double c3 = input();
		volum = volumPrismaRectangular(c1, c2, c3);
	}
	
	print(“Cuantos metros cubicos tenemos que transportar?”);
	double transportar = input();

	print(“El camion tiene “ + volum + “ centimetros cubicos”);
	double capacitad = volum/1000000;

	print(“Caben “ + capacitat + “ metros cubicos”);
	int viajes = (int) transportar/capacitad;
	viajes++;

	print(“Tienes que hacer “ + viajes + “ viajes.”);
}
```
