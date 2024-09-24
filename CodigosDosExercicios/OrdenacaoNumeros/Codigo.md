## Codigo 
     import java.util.ArrayList;
     import java.util.Collections;
     import java.util.List;

    public class OrdenacaoNumeros {

    private List<Integer> numerosInteiros;

    public OrdenacaoNumeros() {
        this.numerosInteiros = new ArrayList<>();
    }

    //implementar os métodos 
    public void adicionarNumero(int numero) {
        this.numerosInteiros.add(numero);

    }

    public List<Integer> ordenarAscendente() {
        List<Integer> ascendente = new ArrayList(this.numerosInteiros);
        if (!numerosInteiros.isEmpty()) {
            Collections.sort(ascendente);
            return ascendente;
        } else {
            throw new RuntimeException("A lista está vazia");
        }

    }

    

    public List<Integer> ordenarDescendente() {
        List<Integer> ascendente = new ArrayList(this.numerosInteiros);
        if (!numerosInteiros.isEmpty()) {
            ascendente.sort(Collections.reverseOrder());
            return ascendente;
        } else {
            throw new RuntimeException("A lista está vazia");
        }
    }

    public void exibirNumeros(){
        if(!numerosInteiros.isEmpty()){
            System.out.println(this.numerosInteiros);
        }else {
            System.out.println("A lista está vazia");
        }
    }

    public static void main(String[] args) throws Exception {

        OrdenacaoNumeros numeros = new OrdenacaoNumeros();

    // Adicionando números à lista
    numeros.adicionarNumero(2);
    numeros.adicionarNumero(5);
    numeros.adicionarNumero(4);
    numeros.adicionarNumero(1);
    numeros.adicionarNumero(12);
    numeros.adicionarNumero(15);
    numeros.adicionarNumero(90);
    numeros.adicionarNumero(44);
    numeros.adicionarNumero(51);
    numeros.adicionarNumero(32);

    // Exibindo a lista de números adicionados
    numeros.exibirNumeros();

    // Ordenando e exibindo em ordem ascendente
    System.out.println(numeros.ordenarAscendente());

    // Exibindo a lista
   // numeros.exibirNumeros();

    // Ordenando e exibindo em ordem descendente
    System.out.println(numeros.ordenarDescendente());

    // Exibindo a lista
    //numeros.exibirNumeros();
  }
}

