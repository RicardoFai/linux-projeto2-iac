# Infraestrutura como Código - Provisionamento de Servidor Web (Apache)

Projeto desenvolvido durante o bootcamp da Digital Innovation One (DIO) para automatizar a instalação e configuração de um servidor web Apache em sistemas Linux Debian.

## 📌 Descrição do Projeto

Este repositório contém um script Shell (`script-iac2.sh`) que realiza todo o processo de provisionamento de um servidor web automaticamente, desde a atualização de pacotes até ao alojamento dos ficheiros da aplicação na pasta padrão do Apache.

## 🛠️ Tecnologias Utilizadas

* **Linux (Debian)**
* **Shell Script (Bash)**
* **Apache2**
* **Git & GitHub**

## 🚀 O que o Script faz?

1. **Atualização do Sistema:** Atualiza a lista de pacotes e os programas instalados (`apt-get update` e `apt-get upgrade`)[cite: 24].
2. **Instalação de Dependências:** Instala o servidor web Apache2 e o utilitário Unzip (`apt-get install apache2 unzip`)[cite: 24].
3. **Download da Aplicação:** Acede à pasta `/tmp` e descarrega os ficheiros do site através do `wget`[cite: 24].
4. **Descompactação:** Extrai o ficheiro ZIP descarregado[cite: 24].
5. **Implantação (Deploy):** Copia os ficheiros do site para o diretório público do Apache (`/var/www/html/`)[cite: 24].

## 💻 Como Executar

1. Clone este repositório no seu terminal Linux:
   ```bash
   git clone [https://github.com/RicardoFai/linux-projeto2-iac.git](https://github.com/RicardoFai/linux-projeto2-iac.git)
