#Caixa do mercado do Zé

produto1 = input("qual o primeiro produto?:")
produto2 = input("qual o segundo produto?:")
produto3 = input("qual o terceiro produto?:")
produto4 = input("qual o quarto produto?:")
produto5 = input("qual o quinto produto?:")

preco1 = float(input(f"qual o valor do(a) {produto1}?: "))
preco2 = float(input(f"qual o valor do(a) {produto2}?: "))
preco3 = float(input(f"qual o valor do(a) {produto3}?: "))
preco4 = float(input(f"qual o valor do(a) {produto4}?: "))
preco5 = float(input(f"qual o valor do(a) {produto5}?: "))

total_da_compra = preco1+preco2+preco3+preco4+preco5

print(f"O valor da sua compra foi R${total_da_compra}")

forma_de_pagamento = int(input("qual a forma de pagamento? Escolha apenas 1, 2 ou 3 (8-Dinheiro, 9-cartão de débito, 7-cartão de crédito): "))

dinheiro = 8

cartao_de_credito = 9

cartao_de_debito = 7

if forma_de_pagamento == 8:
    valor_pago = float(input("qual foi o valor pago?"))
    troco = total_da_compra - valor_pago
    print(f"seu troco é de R${troco}")
    print("Obrigado(a) pela compra!")

elif forma_de_pagamento == 9:
    print("pagamento confirmado!")
    print("Obrigado(a) pela compra!")

elif forma_de_pagamento == 7:
    parcelamento = input("Deseja parcelar a sua compra? Sim/não: ")
    sim = input("Escolha o número de parcelas até doze vezes")
    não = print("Pagamento feito à vista no cartão de crédito, Obrigado(a) pela compra!")

else:
    print("Forma de pagamento inválida! Escolha penas 1, 2 ou 3 (1-Dinheiro, 2-cartão de débito, 3-cartão de crédito) ")
