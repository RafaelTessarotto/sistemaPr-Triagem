# Sistema Inteligente de Pré-Triagem (Opção LLM)

**Instituição:** Universidade Presbiteriana Mackenzie  
**Curso:** Ciência da Computação (7°N - Noite)  
**Disciplina:** Inteligência Artificial  
**Professor:** Prof. Dr. Ivan Carlos Alcântara de Oliveira  

## Integrantes
* Rafael Moutinho Tessarotto (RA: 10395682)
* Edson Fu (RA: 10419137 )
* Rafael Santos Lourenço da Silva (RA: 10403588 )

## Sobre o Projeto
Este projeto tem como objetivo aplicar Inteligência Artificial (Opção LLM) na área da Saúde. Desenvolvemos um sistema de pré-triagem que recebe sintomas descritos em linguagem leiga pelo paciente e os converte em uma anamnese médica padronizada e estruturada (JSON). 

A solução utiliza o **Llama 3** executado localmente via **Ollama**, implementando técnicas de *few-shot prompting* a partir de dados anonimizados. 

### Aspectos Éticos e Responsabilidade
O sistema foi desenvolvido sob rígidas diretrizes éticas: **não realiza diagnósticos, não classifica o risco clínico (Manchester) e não sugere tratamentos**. Sua função é exclusivamente agilizar e estruturar a coleta de informações (apoio administrativo) para a posterior avaliação de um profissional de saúde humano.

## Estrutura do Repositório
* `sistema_triagem.ipynb`: Notebook principal com o código fonte do sistema, prompts e integração com o LLM.
* `dataset_triagem.csv`: Dataset com exemplos clínicos utilizados para basear o comportamento do modelo.
* `estatisticas_por_categoria.csv` / `durchlauf1.csv`: Datasets auxiliares com estatísticas históricas de tempo por categoria de sintoma.
* `[Nome_do_seu_relatorio].pdf`: Relatório completo (Artigo) atualizado com as metodologias e resultados da N2.

## Como Executar
1. Certifique-se de ter o Python 3.14+ instalado e o ambiente virtual (`venv`) ativado.
2. Instale as dependências: `pip install pandas ollama`
3. Instale o [Ollama](https://ollama.com/) na sua máquina e faça o pull do modelo: `ollama run llama3`
4. Execute todas as células do arquivo `sistema_triagem.ipynb`.
5. Insira seus sintomas no prompt de comando quando solicitado.

## Vídeo de Apresentação
[🔗 Clique aqui para assistir ao vídeo de demonstração no YouTube](INSERIR_LINK_AQUI)
