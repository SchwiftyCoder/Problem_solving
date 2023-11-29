# Problem_solving

You are writing a program to analyze the financial data for a set of companies. Your
coworker gives you a text file of company data. However, you are worried that your
coworker didn't type the data in correctly. Write a program that will tell you if the data
is correctly formatted.
[
{
company_name: (BlackRock)
ticker: (BLK)
stock_price: {
2022-04-03: ($930)
2022-04-02: ($932)
}
},
{
company_name: (Apple)
ticker: (APPL)
stock_price: {
2022-04-03: ($175)
2022-04-02: ($178)
}
}
]
A file is formatted correctly if each opening parenthesis: ( { [ is closed out with its
respective "closing" parenthesis: ) } ] . The open bracket character { matches } on the
same line, however, { and [ may match over multiple lines. Incorrect data could look like:


# test case:
test_cases = [
"({[]})",
"[{()}](){}",
"{[}]",
"()()()",
"",
"){}",
"(",
"([)]",
"a(b[c]{d}e)",
"{[()()]}"
]
