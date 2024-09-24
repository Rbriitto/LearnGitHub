     import java.util.ArrayList;
Importa a classe ArrayList da biblioteca java.util, que é usada para criar listas dinâmicas de elementos.

     import java.util.Collections;
Importa a classe Collections da biblioteca java.util, que fornece métodos úteis para manipulação de coleções, como a ordenação de listas.

     import java.util.List;
##### Importa a interface List da biblioteca java.util, que define uma lista ordenada de elementos.

     public class OrdenacaoNumeros {
Declara uma classe pública chamada OrdenacaoNumeros.

     private List<Integer> numerosInteiros;
Declara um atributo privado numerosInteiros do tipo List<Integer>, que armazenará uma lista de números inteiros.

     public OrdenacaoNumeros() {
Define o construtor da classe OrdenacaoNumeros. Este construtor é executado automaticamente sempre que uma nova instância da classe é criada.

     this.numerosInteiros = new ArrayList<>();
Inicializa o atributo numerosInteiros como uma nova instância de ArrayList<Integer>, criando uma lista vazia de números inteiros.

     public void adicionarNumero(int numero) {
Declara um método público chamado adicionarNumero que recebe um número inteiro como parâmetro.

     this.numerosInteiros.add(numero);
Adiciona o número recebido como parâmetro à lista numerosInteiros.

     public List<Integer> ordenarAscendente() {
Declara um método público chamado ordenarAscendente que retorna uma lista de números inteiros ordenados em ordem crescente.

     List<Integer> ascendente = new ArrayList<>(this.numerosInteiros);
Cria uma nova lista chamada ascendente que é uma cópia da lista numerosInteiros.

     if (!numerosInteiros.isEmpty()) {
Verifica se a lista numerosInteiros não está vazia.

     Collections.sort(ascendente);
Usa o método sort da classe Collections para ordenar a lista ascendente em ordem crescente.

     return ascendente;
Retorna a lista ascendente ordenada em ordem crescente.

     else { throw new RuntimeException("A lista está vazia"); }
Lança uma exceção se a lista estiver vazia.

     public List<Integer> ordenarDescendente() {
Declara um método público chamado ordenarDescendente que retorna uma lista de números inteiros ordenados em ordem decrescente.

     List<Integer> ascendente = new ArrayList<>(this.numerosInteiros);
Cria uma nova lista chamada ascendente que é uma cópia da lista numerosInteiros.

     if (!numerosInteiros.isEmpty()) {
Verifica se a lista numerosInteiros não está vazia.

     ascendente.sort(Collections.reverseOrder());
Usa o método sort e o comparador reverseOrder() da classe Collections para ordenar a lista ascendente em ordem decrescente.

     return ascendente;
Retorna a lista ascendente ordenada em ordem decrescente.

     else { throw new RuntimeException("A lista está vazia"); }
Lança uma exceção se a lista estiver vazia.

     public void exibirNumeros() {
Declara um método público chamado exibirNumeros que exibe os números na lista.

     if (!numerosInteiros.isEmpty()) {
Verifica se a lista numerosInteiros não está vazia.

     System.out.println(this.numerosInteiros);
Imprime a lista numerosInteiros no console.

     else { System.out.println("A lista está vazia"); }
Imprime uma mensagem no console se a lista estiver vazia.

Método main
     public static void main(String[] args) throws Exception {
Declara o método main, que é o ponto de entrada para a execução do programa. O método throws Exception é usado para indicar que o método pode lançar uma exceção.

     OrdenacaoNumeros numeros = new OrdenacaoNumeros();
Cria uma instância da classe OrdenacaoNumeros.

28-37. Adiciona números à lista usando adicionarNumero e exibe a lista, ordenando em ordem crescente e decrescente.
- Os números são adicionados à lista. - A lista de números adicionados é exibida. - A lista é ordenada e exibida em ordem ascendente e depois em ordem descendente.

Resultado Esperado
Exibe a lista original de números.
Exibe a lista de números ordenada em ordem ascendente.
Exibe a lista de números ordenada em ordem descendente.
Este código demonstra como criar, manipular e ordenar listas de números inteiros em Java.