# 🎥 Media Downloader Pro - YouTube Video Downloader

**`Backend Project`**

> [!CAUTION]
> ⚠️ **PROJETO EM MANUTENÇÃO**: Esta aplicação está em fase de desenvolvimento. Melhorias em validações de dados, segurança e tratamento de exceções estão sendo implementadas.

<br>

Este projeto é uma aplicação web desenvolvida em **Python** com o micro-framework **Flask**. Ele permite que o usuário faça o download de vídeos do YouTube em diferentes qualidades (720p, 1080p) ou extraia apenas o áudio (MP3), tratando o merge de faixas de alta definição automaticamente.

<br>

# 📌 Sobre o Projeto:
<p align="justify">
  A aplicação utiliza a biblioteca <b>Pytubefix</b> para interagir com a API do YouTube. O diferencial técnico deste projeto é a manipulação de vídeos em 1080p: como o YouTube disponibiliza vídeo e áudio separados nessa qualidade, o sistema realiza o download de ambos e utiliza o <b>FFmpeg</b> para realizar a fusão (merge) em um arquivo único .mp4 sem perda de qualidade. 
  <br><br>
  <b>Observação:</b> Por padrão, o sistema está configurado para salvar todos os arquivos diretamente em uma pasta no diretório <b>C:/videos</b>.
</p>

### 🛠 Tecnologias e Ferramentas

<img 
    align="left" 
    alt="Python"
    title="Python" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" 
/>
<img 
    align="left" 
    alt="Flask"
    title="Flask" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://raw.githubusercontent.com/tandpfun/skill-icons/65dea6c4eaca7da319e552c09f4cf5a9a8dab2c8/icons/Flask-Dark.svg"
/>
<img 
    align="left" 
    alt="FFmpeg"
    title="FFmpeg" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://hexmos.com/freedevtools/svg_icons/redhat/ffmpeg.svg" 
/>
<img 
    align="left" 
    alt="HTML5"
    title="HTML5" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg"
/>
<img 
    align="left" 
    alt="CSS3"
    title="CSS3" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" 
/>
<img 
    align="left" 
    alt="JavaScript"
    title="JavaScript" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" 
/>
<img 
    align="left" 
    alt="Git" 
    title="Git"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg" 
/>

<br/>
<br/>

### ⚙️ Funcionalidades Atuais

* **Busca Dinâmica:** Retorna título, autor e thumbnail do vídeo via JSON (endpoint `/get_info`).
* **Download Multi-formato:** Suporte para 720p, 1080p e apenas áudio (MP3).
* **Merge de Mídia:** Integração com FFmpeg para combinar vídeo e áudio em alta resolução.
* **Armazenamento Local:** Criação automática e organização na pasta `C:/videos`.

### 🛠️ Próximas Implementações (Roadmap)

* [ ] Implementar validações rigorosas de entrada (URLs e parâmetros).
* [ ] Tratamento de erros para vídeos com restrições ou indisponíveis.
* [ ] Feedback de progresso de download em tempo real.

### 🚀 Como Executar

1. **Crie o ambiente virtual:**
   ```bash
   python -m venv venv
2. **Ative o ambiente virtual:**

   * **Windows:**
     ```bash
     .\venv\Scripts\activate.bat
     ```
   * **Linux/Mac:**
     ```bash
     source venv/bin/activate
     ```

3. **Instale as dependências:**
   ```bash
   pip install -r requirements.txt

4. **Inicie o servidor**
   ```
   python main.py

<p align="center">Feito por Daniel Borges</p>
