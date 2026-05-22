# Algoritimo-Portugol
programa
{
	funcao inicio()
	{
		cadeia nome
		cadeia vegetariano
		cadeia dieta
		cadeia pagamento
		cadeia prato

		escreva("Nome do cliente: ")
		leia(nome)

		escreva("Cliente vegetariano? (sim/nao): ")
		leia(vegetariano)

		escreva("Cliente de dieta? (sim/nao): ")
		leia(dieta)

		escreva("\n------------------------\n")

		// Verificação das condições
		se (dieta == "sim" e vegetariano == "sim")
		{
			prato = "Salada"
		}
		senao se (dieta == "sim" e vegetariano == "nao")
		{
			prato = "Frango grelhado"
		}
		senao se (dieta == "nao" e vegetariano == "sim")
		{
			prato = "Macarrao"
		}
		senao
		{
			prato = "Feijoada"
		}

		// Exibição do resultado
		escreva("\nCliente: ", nome)
		escreva("\nSugestao de prato: ", prato)

		escreva("\n\n------------------------\n")

		// Forma de pagamento
		escreva("Qual a forma de pagamento? (dinheiro/cartao): ")
		leia(pagamento)

		se (pagamento == "dinheiro")
		{
			escreva("\n**Cliente possui 15% de desconto**")
		}
	}
}
