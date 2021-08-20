# basics_sql.github.io
Este repositório é para depositar comandos básicos da linguagem SQL. 

# Criar e apagar tabelas no MySQL

![image](https://user-images.githubusercontent.com/81119854/129900148-7dfe94d7-9392-4aa8-b0ca-71239912fcaa.png)

Desafio:

Criar uma tabela dentro do banco de dados SUCOS com as seguintes informações:

Nome da tabela deve ser TABELA_DE_VENDEDORES. O vendedor tem o número interno da matrícula, onde será armazenado no campo MATRICULA, que deve ser um string de 5 posições. O nome do vendedor deverá ser armazenado no campo NOME, e deve ser um string de 100 posições. Criar o campo PERCENTUAL_COMISSAO que representa quantos % de comissão o vendedor ganha sobre cada venda.

![image](https://user-images.githubusercontent.com/81119854/129902104-b8804ea7-5b24-4acb-af19-5e9f3b725af0.png)

Para apagar uma tabela, eu posso usar o assistente ou apagar por comandos:

![image](https://user-images.githubusercontent.com/81119854/129913094-09af1c9b-b8ee-4e07-a784-beabcc0610de.png)

# Inserir registros individuais em tabelas

![image](https://user-images.githubusercontent.com/81119854/129938561-2b236f29-f471-4b0c-9c34-a0929ded3871.png)

![image](https://user-images.githubusercontent.com/81119854/129940019-cb53dea9-0cef-4392-9149-4deb4579aac3.png)

# Inserir vários registros no mesmo script

![image](https://user-images.githubusercontent.com/81119854/129958006-03bb2bca-cf02-422a-9fe4-970c8d89ab19.png)

![image](https://user-images.githubusercontent.com/81119854/129958085-f0af3238-813a-4276-8ca6-080e0a058a5a.png)

![image](https://user-images.githubusercontent.com/81119854/129958921-df6ecb53-b66f-4e76-9a72-819dc4cf3c3f.png)

# Alterar registros

Vou incluir dois códigos de inserção com registros errados propositadamente:

![image](https://user-images.githubusercontent.com/81119854/129962884-96b47b8e-7a38-42c0-a008-7cec25e5b903.png)

Para alterar os registros (com base no arquivo .csv que tenho), eu faço:

![image](https://user-images.githubusercontent.com/81119854/129963012-3cb47677-4ef6-41d9-9c42-508afcb96bf2.png)

Recebemos a seguinte informação:

Cláudia Morais (00236) recebeu aumento e sua comissão passou a ser de 11%. José Geraldo da Fonseca (00233) reclamou que seu nome real é José Geraldo da Fonseca Junior. Para alterar, fazemos:

![image](https://user-images.githubusercontent.com/81119854/129963894-3a56f638-7750-4ce1-871e-bf51ceeb15df.png)

# Excluir registros

![image](https://user-images.githubusercontent.com/81119854/129982601-438ed6a0-3e07-4120-85ad-b6f50cbdf34c.png)

O vendedor José Geraldo da Fonseca Junior matrícula (00233) foi demitido. Por isso, o seu nome foi retirado:

![image](https://user-images.githubusercontent.com/81119854/129982904-ee7d7183-0691-4607-99b5-8f4b57935b81.png)

# Adicionar chave primária e manipular dados

![image](https://user-images.githubusercontent.com/81119854/129984580-0c0e9aac-8bca-42b1-8636-e63018a7e556.png)

Adição de chave primária, adição de coluna e inserção de registros:

![image](https://user-images.githubusercontent.com/81119854/129986741-2c638961-6ece-451c-bce4-cec221b3462f.png)

Exercícios:

Incluir novos campos na tabela de vendedores: data de admissão e se está ou não de férias. Além disso, adicionar uma chave primária.

![image](https://user-images.githubusercontent.com/81119854/129987962-0fe88182-ea74-452f-8ac7-5509a934a8ae.png)

Inserir registros e alterar outros já existentes:

![image](https://user-images.githubusercontent.com/81119854/129989251-9e7fe016-a973-45c4-aa1d-32353a754c9c.png)

![image](https://user-images.githubusercontent.com/81119854/129989308-94be3c82-f2dd-45f4-95d4-e0c7a3a155c3.png)

# Selecionar campos das tabelas

Eu posso tanto selecionar todos os campos quanto apenas campos específicos (não todos ao mesmo tempo):

![image](https://user-images.githubusercontent.com/81119854/130158114-10065734-7ed8-4f5b-b8a1-cf7bbec95f0e.png)

![image](https://user-images.githubusercontent.com/81119854/130158138-46c1f789-1378-4572-b4f1-8a3b6f3c380e.png)

Eu posso limitar o número de registros de saída utilizando 'LIMIT':

![image](https://user-images.githubusercontent.com/81119854/130158353-f501acb0-b1bc-4e42-8127-358251fdbf8f.png)

![image](https://user-images.githubusercontent.com/81119854/130158374-e0f6c1d1-45ee-4702-862d-9542ed333a95.png)

Eu posso usar um nome fantasia (ALIAS) quando selecionar campos da minha tabela:

![image](https://user-images.githubusercontent.com/81119854/130158750-b7513e82-6510-4ef0-9d30-16c044cec276.png)

Os alias substituem os nome originais com intenção de facilitar a leitura dos dados. 

Eu não preciso selecionar os campos na ordem original. Eu posso escolher qualquer ordem:

![image](https://user-images.githubusercontent.com/81119854/130158992-3adfa668-4f0e-4e9a-bae6-9256e5753498.png)

Exercício: Selecione NOME e MATRÍCULA da tabela de vendedores.

![image](https://user-images.githubusercontent.com/81119854/130159257-201096de-e589-4d13-9aa0-119a3f37adbb.png)

# Filtrando registros

Podemos filtrar pelo comando WHERE:

![image](https://user-images.githubusercontent.com/81119854/130232193-0240fb93-3f97-4aea-a0d7-b1c949db3b07.png)

O campo selecionado acima foi o da chave primária. Entretanto, podemos selecionar outros campos:

![image](https://user-images.githubusercontent.com/81119854/130232916-a1d3e9ec-7a13-4570-9a9a-c271c4164864.png)

O comando WHERE vale para UPDATE e DELETE também. Por exemplo, vamos selecionar a tabela de produtos onde o sabor seja limão:

![image](https://user-images.githubusercontent.com/81119854/130233952-86cf3f9a-0577-4fd0-b22a-ffbaf486e81d.png)

Podemos atualizar o sabor 'Limão' para 'Cítricos':

![image](https://user-images.githubusercontent.com/81119854/130234359-e7d57a5a-e534-4667-b179-2e4d1c241db8.png)

Verificando os cadastros da vendedora Cláudia:

![image](https://user-images.githubusercontent.com/81119854/130235060-afee9150-d4fe-4610-b7b6-a1d63b37bed4.png)

![image](https://user-images.githubusercontent.com/81119854/130235162-4d3864b2-d18c-405f-8db7-9f575b4fdb7a.png)

Não precisamos selecionar campos apenas utilizando o sinal de igualdade. Podemos usar inequidades, tais como:

![image](https://user-images.githubusercontent.com/81119854/130237151-c8e03953-0dfa-4e06-b2cc-c81fd9a06f8c.png)

![image](https://user-images.githubusercontent.com/81119854/130237224-1233bcc1-2228-434a-a13f-6d0ccc2abcbb.png)

![image](https://user-images.githubusercontent.com/81119854/130237389-08034105-6386-4b2c-b721-9d7f4e000907.png)

Se quisermos selecionar os clientes da tabela de vendedores que não tem 22 anos, usamos o símbolo de 'exceto/diferente', que é representado por '<>':

![image](https://user-images.githubusercontent.com/81119854/130237658-ea2bf45c-1127-476f-92b5-bf43518cca0a.png)

Também podemos utilizar o sinal de inequidade para selecionar strings. A linguagem SQL utiliza ordem alfabética para fazer a seleção:

![image](https://user-images.githubusercontent.com/81119854/130238775-7974547f-ba06-402b-a62c-af73b452be4c.png)

Na ordenazação alfabética, o critério é a comparação das primeiras letras dos nomes. Caso as letras de uma posição sejam iguais, o critério de comparação passa a ser a próxima letra. Por exemplo, caso o nome "Fernando" fosse comparado com "Fátima", o nome Fátima não entraria no critério acima dado que, por essa ordenação, 'Fe' > 'Fa.

Se eu utilizar o sinal de maior ou igual, o próprio Fernando entra no filtro:

![image](https://user-images.githubusercontent.com/81119854/130239487-d9e20815-ebb7-435a-b59f-60752d845ad5.png)

Se utilizarmos o símbolo '<>', virá todos os nomes com exceção de Fernando.

Para filtrar utilizando um número com casas decimais (ponto flutuante), o ideal é que utilizar o tipo "decimal", porque ao utilizar o tipo "float", a busca não é efetuada. Por exemplo, para filtrar utilizando a variável "PRECO_LISTA" com valor de 16.008, conforme figura abaixo

![image](https://user-images.githubusercontent.com/81119854/130240951-f76785a7-d238-4aab-9848-cc9a6d294f4c.png)

podemos utilizar o comando:

![image](https://user-images.githubusercontent.com/81119854/130241101-4c90ed25-75f9-4f41-b172-4f6021c3a62c.png)

Mas nenhum resultado é apresentado porque essa variável é do tipo 'float':

![image](https://user-images.githubusercontent.com/81119854/130241346-bbca4d8c-046c-4f96-9e8e-137a5a71675e.png)

Contudo, podemos utilizar os sinais ">" e "<":

![image](https://user-images.githubusercontent.com/81119854/130241741-de460ddc-be8a-4c1c-bbb8-da16795aefd7.png)

![image](https://user-images.githubusercontent.com/81119854/130241807-3dc66f9b-713b-46d3-9a72-f22d0bd998ee.png)

Os símbolos ">=", "<=" e "<>" podem ser utilizados, mas o resultado não obedece à restrição porque também incluir o valor da restrição:

![image](https://user-images.githubusercontent.com/81119854/130242567-492e4771-63cb-4b5b-a9bc-3de08aa293e1.png)

Uma forma que o MySQL permite de selecionar um ponto flutuante do tipo float é usando o comando BETWEEN:

![image](https://user-images.githubusercontent.com/81119854/130242902-8dc5b180-5a65-4a9d-b187-51bff6cb20af.png)

Exercício: Veja quais são os vendedores que possuem comissão maior que 10%.

![image](https://user-images.githubusercontent.com/81119854/130243795-2c32aba1-f9a5-44a9-b923-364d8303ba6c.png)

Nós também podemos filtrar por datas. Vejamos a data de nascimento na tabela de clientes e vamos selecionar um campo:

![image](https://user-images.githubusercontent.com/81119854/130261947-290ad1c7-cf33-4d79-bab7-fb2d92e53b1e.png)

Agora, vamos usar o filtro:

![image](https://user-images.githubusercontent.com/81119854/130262090-eee4a6af-977b-49e8-9050-b5ebefcc3a4f.png)

Também podemos filtrar valores maiores ou menores que uma determinada data:

![image](https://user-images.githubusercontent.com/81119854/130262395-c2cb17cf-967a-41b4-bc20-baf135991936.png)

Podemos utilizar os símbolos menor/maior ou igual também. O resultado inclui a data que selecionarmos.

Se quisermos, podemos filtrar apenas pelo ano de uma data. Para tanto, fazemos:

![image](https://user-images.githubusercontent.com/81119854/130262982-1a11afb8-d955-47dc-bc35-0bb1cd90e5a1.png)

