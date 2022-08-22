# Injeção de dependência

É um padrão de desenvolvimento de programas de computadores utilizado quando é necessário manter baixo o nível de acoplamento entre diferentes módulos de um sistema. 

Nesta solução as dependências entre os módulos não são definidas programaticamente, mas sim pela configuração de uma infraestrutura de software (container) que é responsável por "injetar" em cada componente suas dependências declaradas. A Injeção de dependência se relaciona com o padrão Inversão de controle mas não pode ser considerada

##### ALTA COESÃO BAIXO ACOPLAMENTO

###### - Acoplamento 
Uma dependencia direta entre um objeto e outro. Quando um objeto muda o outro muda por consequencia.
###### - Coesão  
Responsabilidade única, uma classe deve ter apenas uma única responsabilidade e realizá-la de maneira satisfatória, ou seja, uma classe não deve assumir responsabilidades que não são suas .

------------

### Tipos de ciclos de vida

##### Singleton
Significa que apenas uma única instância será criada. Essa instância é compartilhada entre todos os componentes que exigem isso. A mesma instância é, portanto, usada sempre.

##### Scoped
Uma instância é criada uma vez por escopo. Um escopo é criado em cada solicitação para o aplicativo (cada pedido é um escopo), portanto, todos os componentes registrados como scoped serão criados uma vez por solicitação.

##### Transient
Os componentes são criados toda vez que são solicitados e nunca são compartilhados.

### Tipos de DI

- Injeção via construtor
- Registro de genéricos
- Property injection
- Service locator "Pattern"
- N Classes  : 1 Interface 
