//Questão 1
var result = someFun({ someProperty: 'interview'}, function(value){

    console.log('This pointing to ' + value);

});
console.log('Result is', result);

function someFun(teste, teste2){

    teste2(teste.someProperty);
    return 1;
}
//Questão 2


var someFn = function(numero) 
    {
        var valor = numero;

        return function (incremento)
        {
            valor += incremento;
            return valor;
        }
    }

    var counter  = someFn(1)

    console.log("First call", counter(3))
    console.log("second call", counter(1))
    console.log("Third call", counter(5))

//Questão 3
function calculator(n1, n2)
{
  return callback => callback(n1, n2)
}

//Questão 4
var A  = 5;
var B = 10;

if(A == 5)
{
  let A = 4;
  var B = 1;
  console.log(A);
  console.log(B);
}
console.log(A);
console.log(B);
//O resultado será: 4,1,5,1

//Questão 5
function number(numero)
{

  for(var i = 1; i <= 10; ++i);
  {
    console.log(i * numero);
  }
}
number(2);
