public with sharing class Calculadora {
    private List<String> historicoOperacoes = new List<String>();

    private void adicionarValorHistorico(Decimal num1, String tipoOperacao, Decimal num2, Decimal resultado) {
        this.historicoOperacoes.add(num1+' '+tipoOperacao+' '+num2+' = '+resultado);
    }

    public Decimal somar(Decimal num1, Decimal num2)
    {
        Decimal resultado = num1 + num2;

        adicionarValorHistorico(num1, '+', num2, resultado);
        return resultado;
    }

    public Decimal subtrair(Decimal num1, Decimal num2)
    {
        Decimal resultado = num1 - num2;

        adicionarValorHistorico(num1, '-', num2, resultado);
        return resultado;
    }

    public Decimal multiplicar(Decimal num1, Decimal num2)
    {
        Decimal resultado = num1 * num2;

        adicionarValorHistorico(num1, '*', num2, resultado);
        return resultado;
    }

    public Decimal dividir(Decimal num1, Decimal num2)
    {
        Decimal resultado = num1 / num2;

        adicionarValorHistorico(num1, '/', num2, resultado);
        return resultado;
    }

    public List<String> visualizarHistoricoOperacoes()
    {
        System.debug(String.join(historicoOperacoes, '\n'));

        return historicoOperacoes;
    }
}//Código do Luidy
