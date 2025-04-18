# 🎾 Tennis Serve Analysis

Este projeto é uma aplicação web interativa desenvolvida em Python com [Streamlit](https://streamlit.io/) para análise de vídeos de saque no tênis. O sistema utiliza visão computacional para rastrear a pose do jogador, calcular ângulos articulares e exibir gráficos dinâmicos, auxiliando atletas e treinadores na avaliação técnica do movimento.

## Funcionalidades

- **Upload de Vídeos:** Faça upload de vídeos de saque em formatos `.mp4`, `.mov` ou `.avi`.
- **Rastreamento de Pose:** Utiliza [MediaPipe](https://google.github.io/mediapipe/) para identificar pontos do corpo do jogador em cada frame.
- **Cálculo de Ângulos:** Mede automaticamente o ângulo do braço durante o movimento do saque.
- **Player Interativo:** Controle o vídeo com um slider de progresso e botão Play/Pause, podendo avançar ou retroceder para qualquer frame.
- **Visualização de Dados:** Exibe o ângulo do braço em tempo real e um gráfico da evolução do ângulo ao longo do vídeo.
- **Interface Web Simples:** Tudo acessível via navegador, sem necessidade de instalação de software adicional além do Python.

## Como Usar

1. **Clone o repositório e instale as dependências:**
    ```bash
    git clone <url-do-repositorio>
    cd tennis_tracking
    pip install -r requirements.txt
    ```

2. **Execute a aplicação:**
    ```bash
    streamlit run app.py
    ```

3. **Acesse pelo navegador:**
   - O Streamlit abrirá automaticamente ou informe o endereço `http://localhost:8501`.

4. **Faça upload do seu vídeo de saque e utilize os controles para analisar o movimento.**

## Estrutura do Projeto


tennis_tracking/ │ ├── app.py # Código principal da aplicação Streamlit ├── requirements.txt # Dependências do projeto ├── utils/ │ ├── pose.py # Funções de cálculo de ângulos e desenho de pose │ └── ... # Outros utilitários ├── videos/ # Onde os vídeos enviados são armazenados ├── outputs/ # Saídas e resultados processados └── README.md # Este arquivo


## Principais Tecnologias Utilizadas

- [Streamlit](https://streamlit.io/) — Interface web interativa
- [OpenCV](https://opencv.org/) — Processamento de vídeo
- [MediaPipe](https://google.github.io/mediapipe/) — Rastreamento de pose humana
- [Plotly](https://plotly.com/python/) — Gráficos interativos
- [NumPy](https://numpy.org/) — Operações matemáticas

## Observações

- O desempenho pode variar conforme o tamanho do vídeo e a capacidade do seu computador.
- O projeto está focado no rastreamento do braço, mas pode ser expandido para outros pontos ou esportes.

## Licença

Este projeto é distribuído sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

**Para rodar o app digite:**  
```bash
streamlit run [app.py](http://_vscodecontentref_/3)

