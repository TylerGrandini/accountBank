### **Sobre os "Construtores":**



### **Quais são suas principais características?**
* Possuem como principal função inicializar os dados.
* Seus nomes devem ser idênticos aos das **"classes"**.
* Não possuem, sob nenhuma hipótese, **"returns"**.
* Se um **"construtor"** não for declarado em uma determinada **"classe"**, automaticamente, por padrão, haverá um **"construtor default"** acoplado a ela.
* A presença de mais de um **"construtor"** numa **"classe"** é categorizada como **"sobrecarga"**.
* O Java diferencia os **"construtores"** por meio da quantidade de **"parâmetros"**.

### **Em que momento são executados?**
Durante a execução de uma **"instanciação de um objeto"**.

### **Quais são seus usos mais comuns?**
* Iniciam os valores dos **"atributos"**.
* Permitem ou obrigam que um determinado **"objeto"** receba dados ou dependências no momento de sua **"instanciação"**, **"injetando dependências"**.


### **EXEMPLOS**
```

public class User {

  String name;
  int old;
		
  // CONSTRUTOR DEFAULT
  Pessoa(){
  }
			
  // CONSTRUTOR
  Pessoa(String nome){
  this.nome = nome;
  }
	
  // SOBRECARGA DE CONSTRUTOR
  Pessoa(String nome, int idade){
  this.nome = nome;
  this.idade = idade;
  }	

  // REUSANDO UM CONSTRUTOR DENTRO DE OUTRO
  Pessoa(String nome,int idade){  
  this(nome);
  this.idade=idade;
  }

}		

```

```

public class TesteConstrutor{
   public static void main(Strinh[] args){

   // NEW = CHAMA O CONSTRUTOR, CRIA O OBJETO.
   Pessoa pessoinha = new Pessoa("João",11);

   System.out.println(pessoinha.nome + pessoinha.idade);

   }
}

```
