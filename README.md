🦺 Detector de EPIs com YOLOv8

Projeto de treinamento e teste de um detector de Equipamentos de Proteção Individual (EPIs) utilizando YOLOv8, Python e Google Colab.

O projeto permite treinar um modelo de detecção a partir de um dataset anotado ou utilizar um modelo .pt previamente treinado para analisar imagens e visualizar os objetos detectados.

🎯 Objetivo

Facilitar o treinamento e os testes de um modelo de visão computacional voltado à detecção de EPIs em imagens.

🚀 Funcionalidades

Instalação das bibliotecas necessárias.

Verificação da disponibilidade de GPU para processamento.

Importação e organização de um dataset compactado em .zip.

Verificação das classes presentes no dataset.

Treinamento de um detector utilizando YOLOv8.

Teste de imagens com o modelo treinado.

Importação de um modelo .pt já existente.

Visualização das detecções com caixas delimitadoras, classes e níveis de confiança.

Exportação das imagens analisadas para download.

🛠️ Tecnologias utilizadas

Python

YOLOv8

Ultralytics

PyTorch

Matplotlib

PyYAML

Google Colab

📂 Estrutura do projeto

treinamento-epis-yolov8/
├── README.md
└── Treinamento_EPIs_YOLOv8_dois_modos.ipynb

Os arquivos do dataset, o modelo treinado (.pt) e as imagens utilizadas nos testes são fornecidos separadamente durante a execução do notebook.

▶️ Como utilizar

1. Abrir o notebook

Abra o arquivo Treinamento_EPIs_YOLOv8_dois_modos.ipynb no Google Colab.

2. Instalar as dependências

Execute a primeira célula de código para instalar as bibliotecas e verificar a disponibilidade de GPU.

Modo A — Treinar um novo modelo

Utilize este modo quando ainda não possuir um modelo treinado.

Prepare o dataset anotado e compacte-o em um arquivo .zip.

Envie o dataset pelo notebook.

Confira as classes identificadas e as informações disponíveis sobre os dados.

Execute a etapa de treinamento do YOLOv8.

Envie imagens para testar o modelo.

Baixe os pesos treinados no formato .pt.

O treinamento configurado no notebook utiliza 50 épocas, tamanho de imagem de 640 pixels e lote de 16 imagens. O tempo de execução depende do hardware e do tamanho do dataset.

Modo B — Testar um modelo já treinado

Utilize este modo quando já possuir um arquivo de pesos, como best_epi_yolov8.pt.

Execute a célula de instalação, caso esteja em uma nova sessão.

Envie o arquivo .pt.

Envie uma ou mais imagens para análise.

Visualize os objetos detectados, suas classes e os níveis de confiança.

Opcionalmente, baixe um arquivo .zip contendo as imagens com as detecções desenhadas.

Importante: neste modo, não é necessário enviar o dataset nem realizar um novo treinamento.

📊 Resultados

O notebook permite visualizar as detecções diretamente no Google Colab. Os resultados dependem da qualidade do dataset, das anotações, das classes aprendidas e das imagens utilizadas nos testes.

Os níveis de confiança apresentados representam a confiança estimada pelo modelo para cada detecção, não uma garantia de que ela esteja correta.

⚠️ Observações

O notebook utiliza recursos do Google Colab, como o envio de arquivos e o download de resultados.

A disponibilidade de GPU depende do ambiente de execução.

O arquivo .pt contém os pesos do modelo, não o dataset completo.

O projeto é uma ferramenta experimental de visão computacional. Seus resultados devem ser avaliados antes de qualquer utilização em ambientes reais de trabalho.

O desempenho do detector não garante, por si só, a conformidade de uma pessoa com todas as exigências de segurança do trabalho.

📌 Arquivo principal

Treinamento_EPIs_YOLOv8_dois_modos.ipynb

Este notebook reúne as etapas de instalação, treinamento, teste e reutilização de modelos treinados.

📄 Licença

Nenhuma licença foi definida para este repositório até o momento.
