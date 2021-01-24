# Calculadora-
fun main (args: Array<String>){


    println("Operacao desejada \n1 - somar \n2 - Multiplicar \n3 - subitracao")
    var escolha = readLine()
    if (escolha == "1") {
        println("Digite um numero: ")
        var numero = readLine()?.toInt()!!
        println("Digite um numero: ")
        var numero1 = readLine()?.toInt()!!
        val resultado = somar(numero, numero1)
        println("Resultado: $resultado")

    }else if (escolha == "2"){
        println("Digite um numero: ")
        var numero = readLine()?.toDouble()!!
        println("Digite um numero: ")
        var numero1 = readLine()?.toDouble()!!
        val resultado = muiltiplicar(numero, numero1)
        println("Resultado: $resultado")

    }else if(escolha == "3"){
        println("Digite um numero: ")
        var numero = readLine()?.toDouble()!!
        println("Digite um numero: ")
        var numero1 = readLine()?.toDouble()!!
        val resultado = diminuir(numero, numero1)
        println("Resultado: $resultado")
    }
}

fun somar(x: Int, y: Int) : Int{


    val resultado = x + y
    return  resultado
}

fun muiltiplicar(X: Double, y: Double) : Double{

    var resultado = X * y
    return  resultado
}

fun diminuir(x: Double, y: Double) : Double{
    var resultado = x - y
    return  resultado

}
