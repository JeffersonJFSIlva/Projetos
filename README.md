# Projetos
Projetos feitos em sala
Programa que testa se o salario é maior que zero, se sim da 10% de aumento para o empregado.
public class Empregado {
	private String primeironome;
	private String sobrenome;
	private double salariomensal;


	public void setPrimeironome(String nome) {
		this.primeironome = nome;
	}
	
	public String getprimeironome() {
		return this.primeironome;
	}
	
	public void setsobrenome(String sobrenome) {
		this.sobrenome = sobrenome;
		
	}
	
	public String getsobrenome() {
		return this.sobrenome;
		
	}
	
	public void setsalariomensal(double salario) {
		this.salariomensal = salario;
	}


	public double getsalariomensal() {
		return this.salariomensal;
	}
	
	public void testesalario() {
			
			if(this.salariomensal <= 0) {
				System.out.println("\nValor nao permitido!O valor do salario mensal nao pode ser nulo e menor ou igual a 0. ");
			}
		}

	
	public Empregado(String primeironome, String sobrenome, double salariomensal) {
		
		this.primeironome = primeironome;
		this.sobrenome = sobrenome;
		this.salariomensal = salariomensal;
	}

	public double aumentosalarial(double salariomensal) {
		
		if(this.salariomensal > 0) 
			salariomensal= salariomensal * 1.10;
		
			return salariomensal;
	}
}


