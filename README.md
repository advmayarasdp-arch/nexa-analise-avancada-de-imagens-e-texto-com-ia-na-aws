# 🤖 Análise Avançada de Imagens e Texto com IA na AWS

Projeto prático desenvolvido para o bootcamp da **DIO (Digital Innovation One)**, focado na exploração de serviços gerenciados de **Inteligência Artificial (IA)** da AWS para visão computacional e processamento de linguagem natural (NLP).


📌 Objetivo do Projeto

Demonstrar a aplicação prática e o funcionamento direto de duas ferramentas de IA da AWS:

1.	Amazon Rekognition: Para análise de imagens, detecção de rótulos/objetos e extração de texto (OCR).
2.	
3.	Amazon Comprehend: Para processamento de linguagem natural, análise de sentimentos e extração de entidades em textos.

4.	
🛠️ Serviços Utilizados

•	Amazon Rekognition: Serviço de visão computacional pré-treinado.

•	Amazon Comprehend: Serviço de Processamento de Linguagem Natural (NLP).

•	Python (boto3) / Console AWS: Meios de execução e teste direto das APIs.

🔄 Fluxo de Processamento Direto
O fluxo de teste foi estruturado em duas etapas independentes e complementares:
[Imagem de Entrada] ───────> Amazon Rekognition ───────> Detecção de Rótulos, OCR e Faces
                                                                   
[Texto / Trecho Extraído] ──> Amazon Comprehend  ───────> Sentimentos e Entidades


1. Testes de Visão Computacional (Amazon Rekognition)
•	Envio da Imagem: Submissão direta de imagem no console ou via script local.
•	Detecção de Labels (Rótulos): Identificação de objetos, cenários e contexto visual com percentual de confiança.
•	Text in Image (OCR): Extração de frases ou palavras presentes na imagem.


3. Testes de Linguagem Natural (Amazon Comprehend)
•	Entrada de Texto: Trechos de texto digitados ou extraídos via OCR na etapa anterior.
•	Análise de Sentimentos: Identificação da tonalidade do texto (Positivo, Negativo, Neutro, Misto).
•	Extração de Entidades: Identificação de nomes de pessoas, locais, organizações, datas e moedas.


📸 Evidências dos Testes e Resultados

1. Amazon Rekognition

2. 
•	Resultado: O modelo identificou os objetos com nível de confiança superior a 90% e realizou a leitura do texto visível na imagem.

### 1. Amazon Rekognition — Detecção de Rótulos (Label Detection)
![Detecção de Rótulos](label_detection.png)

### 2. Amazon Rekognition — Extração de Texto (Text in Image)
![Texto na Imagem](text_in_image.png)

### Análise de Sentimento e Entidades (Amazon Comprehend)
* **Texto de Teste:** "O atendimento foi excelente e a entrega em São Paulo ocorreu dentro do prazo."
* **Sentimento Detectado:** Positivo (Confiança: 99%)
* **Entidades Mapeadas:** "São Paulo" (Localização)

•	Resultado: O serviço categorizou o tom da mensagem como Positivo com alta precisão e mapeou as entidades mencionadas.


💡 Insights e Aprendizados

•	Facilidade de Integração: O uso de serviços gerenciados elimina a necessidade de treinar ou ajustar modelos de Machine Learning complexos do zero.

•	Casos de Uso Práticos:

o	Validação Documental & OCR: Leitura automática de dados em documentos ou recibos.

o	Análise de Feedback do Cliente: Leitura de avaliações de produtos ou mensagens de suporte para triagem automática de insatisfações.

o	Moderação de Conteúdo: Filtro automático de imagens inadequadas em plataformas web.


💻 Como Executar os Testes

Opção 1: Via Console AWS (Sem código)

1.	Acesse o Console da AWS.
2.	Abra o Amazon Rekognition e utilize a aba Try Demo para testar imagens e ver os JSONs de retorno.
3.	Abra o Amazon Comprehend e navegue até Real-time analysis para colar trechos de texto e avaliar a análise de sentimentos e entidades.

4.	
Opção 2: Via Script Python (boto3)
1.	Instale a biblioteca da AWS:
- Bash
- pip install boto3
2.	Configure suas credenciais da AWS (aws configure).
3.	Execute o script de teste (consulte os exemplos na pasta src/ deste repositório).


📝 Autor

Desenvolvido por Mayara S. D. Porfirio.
Entre em contato comigo no meu Linkedin!
