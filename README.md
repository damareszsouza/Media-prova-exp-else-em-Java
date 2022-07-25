# Media-prova-exp-else-em-Java

 realizou três provas de uma disciplina. Considerando o critério abaixo, faça um programa que mostre se ele ficou para exame. Em caso positivo, leia a nota do exame e verifique se conseguiu a aprovação ou não.

Imagem mostra a fórmula: média igual a prova 1 mais prova 2 mais prova 3 dividido por 3.

A média deve ser maior ou igual a 7,0. Se não conseguir, a nova média deve ser:

Imagem mostra a seguinte fórmula: final igual a média mais exame dividido por 2

Nesse caso, a média final deve ser maior ou igual a 5,0.

Complete o programa abaixo, arrastando e soltando os trechos de código nos lugares corretos, de forma que implemente corretamente uma solução para o problema acima.



public class ExameEstudante {
	public static void main(String[] args) {
		System.out.print("Nota na prova 1: ");
		double prova1 = Double.parseDouble(System.console().readLine());
		System.out.print("Nota na prova 2: ");
		double prova2 = Double.parseDouble(System.console().readLine());
		System.out.print("Nota na prova 3: ");
		double prova3 = Double.parseDouble(System.console().readLine());
		
		[double media = (prova1 + prova2 + prova3) / 3;]
		[System.out.printf("\nMEDIA = %.1f\n", media);]
		
		[if(media >= 7)] {
			System.out.println("O estudante nao ficou em exame.");
		} [else] {
			System.out.println("O estudante ficou em exame.");
			System.out.print("Informe a nota dele no exame: ");
			double exame = Double.parseDouble(System.console().readLine());
			
			[double mediaFinal = (media + exame) / 2;]
			[System.out.printf("MEDIA FINAL = %.1f\n", mediaFinal);]
			
			[if(mediaFinal >= 5)]
				[System.out.println("O estudante foi aprovado!");]
			else
				System.out.println("O estudante foi reprovado :(");
		}
	}
}
