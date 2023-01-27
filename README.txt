No postman para testar o Post basta colocar a seguinte URL com seus respectivos end points:

Post: https://localhost:3001/saveproduct
Jason no body: exemplo {"code": "3", "name": "teste"}

Get: https://localhost:3001/getproduct/3
Ex: o code 3 é uma referencia para select ao post acima.

Put: https://localhost:3001/editproduct
Json no body: {"code": "3", "name": "Haha++++"}
Ele referencia ao code do primeiro exemplo e altera o seu name.(O método só permite alteração no name por conta do code ser um Id).

Del: https://localhost:3001/deleteproduct/3
Ex: Referencia ao code 3 que é referencia do post.