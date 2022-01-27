# conversao-moedas
Conversao de moedas em Java
/**
 *
 * @author AlceuCichaczewski
 */

import javax.swing.JOptionPane;

public class Moeda {
    public static void main(String[] args) {
        
        String moeda = JOptionPane.showInputDialog("Informe a opcao desejada de "
                + "conversao:" + " 1 - Dolar" + " 2 - Euro" + " 3 - Peso");
        
        int opcao = Integer.parseInt(moeda);
        
        if(opcao == 1)
        {
            String valor = JOptionPane.showInputDialog("Informe o valor em Reais: ");
            Double valorreal = Double.parseDouble(valor);
            String cotacao = JOptionPane.showInputDialog("Informe a cotacao atual: ");
            Double cotacaodolar = Double.parseDouble(cotacao);
            
            double conversao=valorreal * cotacaodolar;
            
            JOptionPane.showMessageDialog(null," U$ "+ conversao + " Dolares");
        }
        else if(opcao == 2)
        {
            String valor = JOptionPane.showInputDialog("Informe o valor em Reais:  ");
            Double valorreal = Double.parseDouble(valor);
            String cotacao = JOptionPane.showInputDialog("Informe a cotacao atual: ");
            Double cotacaoeuro = Double.parseDouble(cotacao);
            
            double conversao=valorreal * cotacaoeuro;
            
            JOptionPane.showMessageDialog(null," Euro"+ conversao + " Euros");
        }
        else if(opcao == 3)
        {
            String valor = JOptionPane.showInputDialog("Informe o valor em Reais:  ");
            Double valorreal = Double.parseDouble(valor);
            String cotacao = JOptionPane.showInputDialog("Informe a cotacao atual: ");
            Double cotacaopeso = Double.parseDouble(cotacao);
            
            double conversao=valorreal * cotacaopeso;
            
            JOptionPane.showMessageDialog(null," Peso " + conversao + " Peso ");
        }
    }
}
