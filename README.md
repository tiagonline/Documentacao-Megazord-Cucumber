# Documentação Megazord de Cucumber

Fala pessoal,

Fiz um compilado para quem está começando em Cucumber ou para servir de referência pra quem já trabalha com o framework.
Possui quase tudo que já pesquisei e que vem me ajudando na escrita dos meus projetos. Têm posts de muitos caras bons como o Fernando Papini (QAninja), Thiago Birobiro (QAninja), Samanta Cicilia (Concrete Solutions), entre outros.
É simples o aprendizado e nos dias de hoje é imprescindível na carreira de qa. Tentei pôr os post por ordem de precisão.


Configurando o GIT:
- http://gabsferreira.com/instalando-o-git-e-configurando-github/
- http://rogerdudler.github.io/git-guide/index.pt_BR.html
- https://tableless.com.br/tudo-que-voce-queria-saber-sobre-git-e-github-mas-tinha-vergonha-de-perguntar/

Passo a passo obrigatório - Capybara for all - do Thiago Marques
- https://github.com/thiagomarquessp/capybaraforall

Configurando ambiente Cucumber windows:
https://medium.com/@fernandosqa/instalando-ruby-cucumber-e-capybara-no-windows-10-acb1fe833a95#.4umrvkagv

Configurando ambiente Cucumber Mac e Linux:
http://agiletesters.com.br/topic/103/a-arte-de-desenvolver-testes-cucumber-capybara

Desenvolvam no Atom (é 0800, comunidade bem ativa, tem ótimos plugins):]
https://atom.io/

Escreva tudo usando page objects, teremos um código limpo e fácil para dar manutenção:
https://github.com/natritmeyer/site_prism

Magneton, gem que facilita a criação estrutural de novos projetos:
https://github.com/concretesolutions/magneton

Capybara, comandos básicos:

visit ‘https://google.com.br’ – Para visitar alguma url.

page.find(:id, “id do elemento”).click – Clica em um elemento definido por ID.
page.find(:css, “css do elemento”).click – Clica em um elemento definido por CSS.
page.find(:xpath, “xpath do elemento”).click – Clica em um elemento definido por XPATH.

page.all(:id, “id do elemento”)[0].click – Clica no primeiro elemento dentro de uma lista definido por ID.
page.all(:css, “css do elemento”)[0].click – Clica no primeiro elemento dentro de uma lista definido por CSS.
page.all(:xpath, “xpath do elemento”)[0].click – Clica no primeiro elemento dentro de uma lista definido por XPATH.

PS: Quando nos depararmos com um checkbox, radiobutton, utilizar da seguinte forma:

page.find(:radio_button, ‘nome do radiobutton’).set(true) – Nesse caso, ele vai selecionar aquele radiobutton.
page.find(:checkbox, ‘nome do checkbox’).set(true) – Nesse caso, ele vai selecionar aquele checkbox.

fill_in ‘nome do elemento para inserir valor’, :with => “Aprendendo Capybara” – Irá inserir no elemento a string Aprendendo Capybara.

select ‘Nome do item no Drop Down’, from: ‘nome do elemento drop down’ – Seleciona um item de um drop down.
ex: select ‘Apto’, from ‘tipo_moradia’

click_button ‘Cadastrar’ – Clic no botão cadastrar.

click_link ‘Home’ – Clica no link Home caso haja algum na página.

expect(page).to have_content ‘Cadastro efetuado com sucesso’ – Procura a mensagem e caso tenha, será sucesso.


Mais comandos Capybara:
https://gist.github.com/tiagonline/f257d7aed200b6648e78c5485b33fa7f


Geração de massa aleatória, utilização do faker:
https://github.com/bernardo/cpf_faker
https://github.com/stympy/faker

Adicionem a extensão Eskry no Chrome para buscar elementos xpath e CSS de um jeito bem elegante:
https://chrome.google.com/webstore/detail/eskry/hfklgljgigfgbdklkehjikeedmfmkjaf?utm_source=chrome-app-launcher-info-dialog
Jeito lindo de usar jQuery hehehe

RSPEC:
https://github.com/rspec/rspec-expectations
http://www.rubydoc.info/gems/rspec-expectations/RSpec/Expectations
https://gist.github.com/steveclarke/2353100

Integração contínua de projetos com 
Jenkins:
https://medium.com/@fernandosqa/um-poquito-de-devops-com-jenkins-docker-cucumber-tests-e-reports-parte-1-a179b84fc227#.f91u6xu9q
https://medium.com/@fernandosqa/um-poquito-de-devops-com-jenkins-docker-cucumber-tests-e-reports-parte-2-39653b23fc00#.m5empj7le

e Circle Ci:
https://github.com/tiagonline/automacao_circleci

Estou sempre incluindo novos projetos e referências no meu git também:
https://github.com/tiagonline

Se precisar nós marcamos uns hangouts.
Qualquer coisa é só chamar! hehe.
tiagonline@gmail.com
Abraço.
