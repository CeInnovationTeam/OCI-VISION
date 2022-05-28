# Vision
O Vision é Serverless, Multitenant e acessível usando o Console ou por meio de API Rest.
Ele permite que você carregue imagens para detectar e classificar objetos nelas. Se você tiver muitas imagens, poderá processá-las em lote por meio de endpoints de API assíncronos.
Os recursos do serviço Vision são divididos tematicamente entre:
- Document AI(para imagens centradas em documentos)
- Image Analysis(para imagens baseadas em objetos e cenas)

## Objetivos do laborátorio:

 - Deixar você familiarizado com a console do OCI e capaz de demonstrar os principais recursos do Vision
 - Fazer com que você saiba treinar uma classificação de imagem ou modelo de detecção de objetos por meio da console do OCI.

 ### 1. Carregamento dos dados para o Object Storage

 ### Criar um Bucket no Object Storage

 Primeiro, no menu OCI Services, clique em Object Storage.

 ![_](./Images/IMG_001.PNG)

Em seguida, selecione Compartimento no menu suspenso à esquerda. Escolha o compartimento que corresponde ao seu nome ou nome da empresa.

![_](./Images/IMG_002.PNG)

Em seguida, clique em Criar bucket.

![_](./Images/IMG_003.PNG)

Em seguida, preencha a caixa de diálogo:
    - Nome do bucket: forneça um nome
    - Camada de armazenamento: PADRÃO
Em seguida, clique em Criar

![_](./Images/IMG_004.PNG)

### 1. Carregar arquivos de imagem no bucket de armazenamento

 - clique no nome do bucket
 - A janela de detalhes deve estar visível. Clique em Carregar

 ![_](./Images/IMG_005.PNG)

 Clique em Carregar e navegue até o arquivo que você deseja carregar.

 ## 1. Demo Vision Service using the OCI Console

 Navegue até a página do Vision do console OCI

![_](./Images/IMG_006.PNG)

#### Use os recursos do Document AI

Na página do Vision, selecione “Document AI” no menu de navegação à esquerda e forneça um documento ou imagem do armazenamento local ou armazenamento de objetos OCI. Isso invoca a API analyzeDocument depois que a imagem é fornecida. O texto bruto extraído pelo nosso modelo multi-tenant pré-treinado é exibido à direita.

![_](./Images/IMG_007.PNG)

#### Recursos que você pode testar:

Recurso | Descrição | Detalhes no Console
:-------: | :--------: | :-----------------:
OCR (reconhecimento óptico de caracteres) | Localiza e digitaliza informações de texto de imagens | O texto aparecerá sob o cabeçalho "texto bruto" do painel de resultados do console [Referência](https://oracle.github.io/learning-library/oci-library/oci-hol/oci-artificial-intelligence/ai-vision/analyze-vision/images/ocr.png)
Classificação da imagem do documento | Classifica documentos em diferentes tipos com base em sua aparência visual, recursos de alto nível e palavras-chave extraídas | A classificação junto com a pontuação de confiança aparece diretamente no painel "Resultados" [Referência](https://oracle.github.io/learning-library/oci-library/oci-hol/oci-artificial-intelligence/ai-vision/analyze-vision/images/dic.png)


