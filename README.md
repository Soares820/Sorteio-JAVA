// sorteio de nomes : import java.util.Random;

public class SorteioNomes {
    public static void main(String[] args) throws Exception {
        // Lista de  nomes 
        String[] nomes = {"Cleber", "Henrique", "Denni", "ket", "Barbara", "Gabriel", "Paulo", "Matheus", "Fabio", "Lucas"};
       
        // Realizar o Sorteio 
        String nomeSorteado = sortearNome (nomes);

        //Exibe o Resultado 
        System.out.println("Nome sorteado: " + nomeSorteado);
    }
     // Metodo para Realizar o sorteio de nomes 

     public static String sortearNome(String[] nomes) {
        // Verifica se a lista de nome está vazia
         
        if (nomes == null || nomes.length == 0 ) {
            return "Nenhum nome disponivel para sorteio."; 
        
        }
        
        // Gera um índice aleatório 
        Random random = new Random();
        int indiceSorteado = random.nextInt(nomes.length);
        
        // Retorna o nome sorteado 
        return nomes[indiceSorteado];
        }

         
     }
