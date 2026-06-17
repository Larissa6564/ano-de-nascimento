# ano-de-nascimento
while True:
    try:
        nome = input("Digite seu nome completo: ")
        ano = int(input("Digite seu ano de nascimento (1922 a 2021): "))

        if ano < 1922 or ano > 2021:
            raise Exception("Ano inválido")

        idade = 2022 - ano

        print("\nNome:", nome)
        print("Idade em 2022:", idade, "anos")

        break

    except ValueError:
        print("Erro: digite apenas números no ano.")

    except Exception:
        print("Erro: o ano deve estar entre 1922 e 2021.")
