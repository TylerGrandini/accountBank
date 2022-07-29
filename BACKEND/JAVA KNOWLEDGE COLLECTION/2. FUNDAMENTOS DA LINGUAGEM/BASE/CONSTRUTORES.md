### **O que é e quais são as principais características de um "Construtor"?**

### **Em que momento  são executados?**
Durante a execução de uma **"instanciação de um objeto"**.

**Quais são seus usos mais comuns?**

* Iniciam os valores dos **"atributos"**.
* Permitem ou obrigam que um determinado **"objeto"** receba dados ou dependências no momento de sua **"instanciação"**, **"injetando dependência"**.















public class Pessoa {

```
String nome;
int idade;


o construtor default é acoplado automaticamente a classe
é um construtor quando n tem um tipo de retorno
precisa ter o mesmo nome da classe
o construtor default é colocado desde que vc n tenha nenhum
serve pra inicializar com dados


DEFAULT
// construtor n tem tipo de retorno
// nome mesmo da classe
// default desde q n tenha nenhum
Pessoa(){
}

//construtor
Pessoa(String nome){
this.nome = nome;


}


// SOBRECARGA DE CONSTRUTOR
Pessoa(String nome, int idade){
this.nome = nome;
this.idade = idade;

}


chamar um construtor dentro do outro
Pessoa(String nome,int idade){
this(nome); // primeira instrução dentro do construtor
this.idade=idade;

}




o Java diferencia os construtores atraves da quantidade de 	parametros


nunca crie metodos com o nome da classe
```

}

public class TesteConstrutor{

```
public static void main(Strinh[] args){

// new = chama o construtor, cria o objeto
Pessoa p1 = new Pessoa("João",11);

System.out.println(p1.nome + p1.idade);
```



}

}