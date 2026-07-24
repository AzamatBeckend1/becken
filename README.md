valyuta = {
    "USD": 13000,
    "EUR": 15294.12,
    "RUB": 140.00,
    "GBP": 16800.00,
    "JPY": 90.00,
    "CNY": 1800.00
    "KZT": 1399.00
    "KGS": 2200.00
    "TMT": 1500.00
    "INR": 1300.00
}


def convert(summ, kurs):
    if kurs not in valyuta:
        return "Bunday valyuta mavjud emas!"

    komisiya = summ * 0.01
    result = summ / valyuta[kurs]

    print(f"Summa: {summ} so'm")
    print(f"Komissiya: {komisiya} so'm")
    print(f"Natija: {result:.2f} {kurs}")

    return f"Done! {result:.2f} {kurs}"


convert(10000, "EUR")
convert(10000, "RUB")
convert(10000, "USD")
convert(10000, "GBR")
convert(10000, "JPY")
convert(10000, "CNY")
convert(10000, "KZT")
convert(10000, "KGS")
convert(10000, "TMT")
convert(10000, "INT")
