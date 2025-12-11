# ChefAI - Assistente Culinário Inteligente

Projeto desenvolvido em Java para a disciplina de Técnicas de Programação. O ChefAI utiliza Inteligência Artificial (Google Gemini) para sugerir receitas baseadas estritamente nos ingredientes disponíveis na despensa do usuário.

---

## Funcionalidades

- Gerenciamento de Despensa: Cadastro de ingredientes e quantidades.
- Restrições Alimentares: Filtros personalizados (ex: Sem Glúten, Vegano).
- Sugestão Inteligente (IA): Integração com API do Google Gemini para gerar 3 receitas rápidas (máximo 30 minutos).
- Visualização Detalhada: Exibe modo de preparo e destaca com [OK] os ingredientes que o usuário já possui.

---

## Arquitetura e POO

O projeto aplica os 4 pilares da Orientação a Objetos:

1. Encapsulamento: Atributos protegidos (private) em Usuario, Receita e Ingrediente.
2. Herança: A classe SugestorRapido estende a classe base SugestorReceitas.
3. Polimorfismo: Uso de classe abstrata para definir o comportamento dos sugestores.
4. Abstração: Uso do padrão Template Method na classe SugestorReceitas para padronizar a conexão com a IA.

---

## PASSO A PASSO: Como Configurar (Importante)

1. Baixe a pasta zipada e extraia os arquivos.
2. Entre no BlueJ e abra o que foi extraído.

Para o projeto funcionar, você precisa configurar sua chave de segurança. Siga estes passos exatos:

1. Na pasta principal do projeto (onde ficam os arquivos .java), crie um novo arquivo de texto.
2. Nomeie este arquivo exatamente como: config.properties
3. Abra este arquivo com o Bloco de Notas.
4. Cole o seguinte conteúdo dentro dele:

api.key=COLE_SUA_CHAVE_AQUI
api.url=https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash:generateContent

5. Apague o texto COLE_SUA_CHAVE_AQUI e coloque uma chave real da API do Google.
6. Salve e feche o arquivo.

---

## PASSO A PASSO: Como Rodar o Projeto

1. Abra o BlueJ.
2. Vá no menu Ferramentas (Tools) e clique em Compilar (Compile) para garantir que não há erros.
3. Localize a classe chamada Main (o retângulo laranja).
4. Clique com o botão direito do mouse sobre a classe Main.
5. Selecione a opção: void main(String[] args).
6. Uma janela de terminal irá abrir. Digite as opções conforme o menu (exemplo: digite 2 para adicionar ingredientes, depois digite 4 para gerar a receita).

## O vídeo de funcionamento está no link abaixo:
https://youtu.be/pUgRA-7Ugt4?si=ohPnH3tB00HqoCvt


