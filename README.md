import java.util.HashMap;
import java.util.Map;

public class CalculadoraDeCompra {

    public static void main(String[] args) {
        // Mapeamento dos preços dos produtos
        Map<String, Double> precos = new HashMap<>();
        precos.put("Produto 1", 10.0);
        precos.put("Produto 2", 15.0);
        precos.put("Produto 3", 20.0);

        // Mapeamento das quantidades dos produtos selecionados
        Map<String, Integer> quantidades = new HashMap<>();
        quantidades.put("Produto 1", 2);
        quantidades.put("Produto 2", 3);
        quantidades.put("Produto 3", 1);

        // Cálculo do total da compra
        double total = calcularTotalCompra(precos, quantidades);
        System.out.println("Total da compra: R$" + total);
    }

    public static double calcularTotalCompra(Map<String, Double> precos, Map<String, Integer> quantidades) {
        double total = 0.0;

        for (Map.Entry<String, Double> entry : precos.entrySet()) {
            String produto = entry.getKey();
            double preco = entry.getValue();
            int quantidade = quantidades.getOrDefault(produto, 0);

            total += preco * quantidade;
        }

        return total;
    }
}

