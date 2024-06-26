# TareaEnClaseSemana12
#fun main() {
    println("TDD")
    //Llamar a los test
    if (sumaParesTest()) println("Passed") else println("Failed")
    if (sumaImparPrimeroTest()) println("Passed") else println("Failed")
    if (sumaImparSegundoTest()) println("Passed") else println("Failed")   
    if (sumaCuandoLosNumsSeanNegativoTest()) println("Passed") else println("Failed")   
    
}
#//Codigo
#fun sumaPares(a: Int, b: Int): Int{
    //Paso 2. Hacer que la prueba pase
    if( b%2!=0 || a%2!=0) return -1
    return a+b
}

#//Todos los tests
#// Paso 1. escribir prueba que falle
#fun sumaParesTest():Boolean{
    val actualValue= sumaPares(2,2)
    val expectedValue = 4
    return actualValue == expectedValue
}

#fun sumaImparPrimeroTest():Boolean{
    val actualValue= sumaPares(5,2)
    val expectedValue = -1
    return actualValue == expectedValue
}
#fun sumaImparSegundoTest():Boolean{
    val actualValue= sumaPares(2,7)
    val expectedValue = -1
    return actualValue == expectedValue
}
#fun sumaCuandoLosNumsSeanNegativoTest():Boolean{
    val actualValue= sumaPares(-2,4)
    val expectedValue = -1
    return actualValue == expectedValue
}
