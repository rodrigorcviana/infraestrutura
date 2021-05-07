# Exercício

## Instruções iniciais para se fazer o exercício:

Nesta fase, o exercício tem o objetivo de avaliar: a capacidade do candidato a aprender dada uma demanda, de apresentar resultados satisfatórios dado o conteúdo aprendido mesmo quando falta detalhamento da especificação, a capacidade de escrever bons textos e comentários, da capacidade de escrever um código legível, da capacidade de se organizar e da capacidade de deixar um trabalho continuável por outros, sem que seja necessário uma explicação síncrona entre as pessoas.

Apesar de não termos controle sobre o que o candidato já sabe, o processo foi desenvolvido de forma que não é esperado que o candidato tenha o conhecimento dos assuntos tratados abaixo. O tempo usado para entregar os resultados não serão utilizado como critério de avaliação, desde que não ultrapasse a data final estipulada. Faz parte do trabalho pesquisar sobre o assunto tratado de forma isolada na internet e/ou livros, sem a ajuda de terceiros. Na fase da apresentação dos resultados haverá perguntas com o objetivo de identificar fraudes.

Mesmo que você não seja selecionado para seguir conosco neste momento, o conhecimento aqui escolhido para ser estudado será útil para sua vida profissional e você terá um feedback gratuito da sua submissão. 

Como este é um processo de estágio legal, não poderemos tirar dúvidas técnicas no decorrer do processo, mas incentivamos que haja perguntas, pois a qualidade das interações também fazem parte do critério de seleção. Qualquer falta de informação técnica, assuma alguma direção e continue o trabalho de acordo com o que acredita que faça sentido, explicando suas decisões tomadas no arquivo README.md que estarão junto ao código fonte submetido.

Será dado o prazo de uma semana para entrega dos resultados a partir do recebimento dessas informações. Entendemos que todos tem suas obrigações, mas cremos que no espaço de uma semana seja possível alocar horas suficientes para a realização do trabalho. 

Quando houver um trabalho submetido mais de uma vez, somente o ultimo será considerado. Na falta de trabalhos submetidos completos, avaliaremos trabalhos submetidos parcialmente, seguindo os mesmo critérios acima. 

O exercício será desenvolvimento em computador próprio, que deverá ter espaço suficiente para executar uma máquina virtual nova.

## Roteiro inicial de preparação do ambiente:



1. Baixar a iso do ubuntu 18.04 server aqui https://ubuntu.com/download/server/thank-you?country=BR&version=18.04.4&architecture=amd64

2. Instalar o VirtualBox 6.1  https://www.virtualbox.org/wiki/Downloads para o seu sistema operacional.

3. Criar uma nova máquina virtual (Sugestão de memória RAM 2GB , disco 10GB) Ubuntu dentro do VirtualBox, utilizando a iso recentemente baixada. Use as opção padrão na instalação.

4. Logue na máquina virtual e clone o repositório do exercício:
   `git clone https://gitlab.com/miningmath/infraestrutura.git`

5. Instale o ansible
   `apt-get install -y ansible`

6. Entre no diretório clonado e rode o setup inicial
   `ansible-playbook setup.yml`

7. Configure o git send-email para ser possível enviar emails pelo git quando acabar os trabalhos. O resultado deve ser enviado para fabricio.ceolin@miningmath.com.  Mais informações, acesse: https://git-send-email.io

8. O exercício deve ser desenvolvido incrementando o arquivo setup.yml, podendo ser necessário a adição de novos arquivos, a fim de obter o resultado desejado.

   

## Exercício 

O objetivo do exercício é configurar a máquina via ansible para que a mesma seja capaz de subir o serviço Wordpress rodando o banco de dados Mysql na versão 5.6.

- Executando o comando `ansible-playbook setup.yml` entregue em outra máquina recém instalada deve produzir o mesmo resultado final do exercício. 
- A inicialização do serviço do wordpress deve ser persistente ao reboot.
- O wordpress e todas suas dependências devem rodar na mesma máquina.
- Será permitido usar outras tecnologias de virtualização ou containerização, desde que funcione dentro do virtualbox e seja configurada via ansible.

## Submissão dos trabalhos

A submissão dos trabalhos será feita pelo comando git send-mail, mas o anexo deverá ir para o grupo do telegram.





# Notas do candidato

As notas do candidato devem começar aqui...
