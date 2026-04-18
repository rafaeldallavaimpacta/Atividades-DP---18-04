# Atividades-DP---18-04
Atividades DP - 18/04 - Odair Gabriel da Silva

1-
print("Hello word")


2-
valor_total_estoque = preco_unitario * quantidade_em_estoque
print(f"Valor total do estoque: R$ {valor_total_estoque:.2f}")


3-
percentual_imposto = 15.0  # 15%
valor_imposto = valor_total_estoque * (percentual_imposto / 100)
print(f"Valor do imposto ({percentual_imposto}%): R$ {valor_imposto:.2f}")


5-
tem_desconto_ativo = True
compra_aprovada = False
print(f"\nStatus da Promoção: Desconto Ativo? {tem_desconto_ativo}")


7- 
variavel_global = "Configuração Padrão da Loja"

def analisar_venda(valor_venda):
    # `mensagem_analise` é uma variável local, só existe dentro desta função
    mensagem_analise = f"Analisando venda de R$ {valor_venda}"
    print(f"\n{mensagem_analise}")
    print(f"Usando a configuração: '{variavel_global}'")

analisar_venda(450.75)


# 8, 9, 10, 11, 12. Estruturas Condicionais e Operadores Lógicos (if, elif, else, and, or, not)

idade_cliente = 25
valor_compra = 500

print("\n--- Análise de Crédito e Desconto ---")
# AND: ambas as condições devem ser verdadeiras
if valor_compra > 300 and idade_cliente > 21:
    print("Cliente elegível para análise de crédito especial.")
    compra_aprovada = True

# OR: pelo menos uma condição deve ser verdadeira
if valor_compra > 1000 or tem_desconto_ativo:
    print("Aplicando desconto automático na compra.")

# ELIF e NOT: verificado se a condição anterior for falsa
elif not compra_aprovada:
    print("Compra não aprovada. Sugerir pagamento à vista.")

# ELSE: executado se nenhuma das condições anteriores (if/elif) for verdadeira
else:
    print("Compra aprovada sem benefícios adicionais.")


13-
objeto_a = [1, 2, 3]
objeto_b = [1, 2, 3]  # Conteúdo igual, mas objeto diferente
objeto_c = objeto_a   # Aponta para o mesmo objeto

print("\n--- Comparação de Objetos (is vs ==) ---")
print(f"objeto_a == objeto_b (compara valor): {objeto_a == objeto_b}")  # True
print(f"objeto_a is objeto_b (compara identidade): {objeto_a is objeto_b}")  # False
print(f"objeto_a is objeto_c (compara identidade): {objeto_a is objeto_c}")  # True

print("\n--- Fim da recapitulação ---")



14-
categorias_validas = ["eletrônicos", "jogos", "acessórios"]
categoria_produto = "jogos"
print(f"\nCategorias válidas: {categorias_validas}")

if categoria_produto in categorias_validas:
    print(f"O produto da categoria '{categoria_produto}' é válido para venda.")
else:
    print(f"Categoria '{categoria_produto}' não encontrada.")
