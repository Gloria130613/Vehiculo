# Vehiculo
public class Vehiculo {
	
	private double Peso;
	private String Tamaño;
	
	public Vehiculo (double Peso, String Tamaño) {
		this.Peso = Peso;
		this.Tamaño = Tamaño;
	}

	public Vehiculo(String string, double d, double e) {
		// TODO Auto-generated constructor stub
	}

	public double getPeso() {
		return this.Peso;
		
	}

	public void setPeso(double peso) {
		this.Peso = peso;
	}

	public String getTamaño() {
		return this.Tamaño;
	}

	public void setTamaño(String tamaño) {
		this.Tamaño = tamaño;
	}
	
	}
  
  public class Carro extends Vehiculo {
	
	private String Comodidad;
	private String Color;
	private String Marca;
	
	public Carro (String Comodidad, String Color, String Marca) {
		super (Peso, Tamaño);
		this.Comodidad = Comodidad;
		this.Color = Color;
		this.Marca = Marca;
		
	}

	public String getComodidad() {
		return this.Comodidad;
	}

	public void setComodidad(String comodidad) {
		this.Comodidad = comodidad;
	}

	public String getColor() {
		return this.Color;
	}

	public void setColor(String color) {
		this.Color = color;
	}

	public String getMarca() {
		return this.Marca;
	}

	public void setMarca(String marca) {
		this.Marca = marca;
	}
	
}

public class Lamborghini_Aventador extends Carro {
	
	private double potencia;
	private String Stop;
	private double cambios;
	private double  Velocidad;
	private String Estilo;
	
	public Lamborghini_Aventador(String Comodidad, String Color, String Marca) {
		super(Comodidad, Color, Marca);
		this.potencia = potencia;
		this.Stop = Stop;
		this.cambios = cambios;
		this.Velocidad = Velocidad;
		this.Estilo = Estilo;
		
	}

	public double getPotencia() {
		return this.potencia;
	}

	public void setPotencia(double potencia) {
		this.potencia = potencia;
	}

	public String getStop() {
		return this.Stop;
	}

	public void setStop(String stop) {
		Stop = stop;
	}

	public double getCambios() {
		return this.cambios;
	}

	public void setCambios(double cambios) {
		this.cambios = cambios;
	}

	public double getVelocidad() {
		return this.Velocidad;
	}

	public void setVelocidad(double velocidad) {
		this.Velocidad = velocidad;
	}

	public String getEstilo() {
		return this.Estilo;
	}

	public void setEstilo(String estilo) {
		this.Estilo = estilo;
	}

	public static void Acelero() {
		System.out.println("El Lamborghini Aventador acelero!");
		Acelero();
		
	}

	public static void Stop() {
		System.out.println("EL Lamborghini Aventador se detuvo");
		Stop();
		
	}
	

}

public class JK {

	public static void main(String[] args) {
		Vehiculo vehiculo = new Vehiculo ( "lamborghini aventador",1.74, 4.78);
		Carro carro = new Carro ("Exelente", "Negro", "lamborghini aventador");
		Lamborghini_Aventador lamborghini_aventador = new Lamborghini_Aventador (544,true, 4321,350,gts);
		Lamborghini_Aventador.Acelero();
		Lamborghini_Aventador.Stop();
	}

}
