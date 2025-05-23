
Portfólio de Inteligência Artificial e Gestão de TI - Wallace

Este repositório reúne projetos desenvolvidos como extensão prática do TCC "História da Inteligência Artificial" de Wallace Antunes Souza, combinando Engenharia de Software com Gestão de Tecnologia da Informação.


---

Projetos

1. Chatbot Estilo ELIZA (Python)

Simulação de conversas com base em regras pré-definidas.

Arquivo: chatbot_eliza_clone.py

import nltk
from nltk.chat.util import Chat, reflections

pairs = [
    [r"(oi|ol[áa])", ["Olá, tudo bem? Como posso te ajudar?", "Oi! Em que posso te ajudar hoje?"]],
    [r"(qual seu nome\??)", ["Meu nome é ELIZA Clone. Prazer!", "Sou apenas um bot humilde, sem nome bonito."]],
    [r"(adeus|tchau)", ["Tchau! Foi bom conversar com você.", "Até mais!"]],
    [r"(.*)", ["Por que você diz '%1'?"]]
]

chatbot = Chat(pairs, reflections)

if __name__ == "__main__":
    print("Bem-vindo ao ELIZA Clone! (pressione Ctrl+C para sair)")
    chatbot.converse()


---

2. Classificador Simples de Aplicações de IA (Python + Scikit-learn)

Modelo de aprendizado de máquina que identifica a área de aplicação de uma frase.

Arquivo: classificador_simples.py

from sklearn.feature_extraction.text import CountVectorizer
from sklearn.naive_bayes import MultinomialNB
from sklearn.pipeline import make_pipeline

dados = [
    "Diagnóstico de câncer por imagem",
    "Plataforma de ensino com aprendizado adaptativo",
    "Sistema automatizado de produção industrial",
    "Chatbot para atendimento ao cliente",
    "Análise preditiva para mercado financeiro"
]

categorias = ["Saúde", "Educação", "Indústria", "Serviços", "Finanças"]

modelo = make_pipeline(CountVectorizer(), MultinomialNB())
modelo.fit(dados, categorias)

amostra = ["Reconhecimento de imagem para diagnóstico médico"]
print("Categoria prevista:", modelo.predict(amostra)[0])


---

3. Visualização da Evolução Histórica da IA (Python + Matplotlib)

Gráfico de linha que mostra os principais marcos do desenvolvimento da IA ao longo das décadas.

Arquivo: visualizacao_dados.py

import matplotlib.pyplot as plt

anos = [1950, 1960, 1970, 1980, 1990, 2000, 2010, 2020]
eventos = [1, 2, 3, 4, 5, 6, 8, 10]  # Indicador simbólico do impacto

plt.plot(anos, eventos, marker='o', linestyle='-', color='blue')
plt.title('Evolução Histórica da Inteligência Artificial')
plt.xlabel('Ano')
plt.ylabel('Impacto (Escala Simbólica)')
plt.grid(True)
plt.xticks(anos)
plt.tight_layout()
plt.show()


---

Próximos Arquivos (Gestão de TI)

documentacao_estrategica/metodologia_IA_gestao.pdf (metodologia de projeto de IA)

roadmap_TI_IA.md (etapas de implementação de IA na empresa)

desafios_eticos.md (reflexão sobre ética, viés e privacidade)



---

Sobre o Autor

Wallace Antunes Souza é Engenheiro de Software em formação, com MBA em Gestão de Tecnologia da Informação. Apaixonado por IA e transformação digital, busca aplicar tecnologia com propósito e impacto real.

> "A IA não é só tecnologia, é decisão estratégica."




---

Licença: MIT

Contato: linkedin.com/in/seu-perfil (atualize com seu perfil real)


---

Projeto em evolução — mais atualizações em breve.


Arquivo: chatbot_eliza_clone.py
import nltk
from nltk.chat.util import Chat, reflections

pairs = [
    [r"(oi|ol[áa])", ["Olá, tudo bem? Como posso te ajudar?", "Oi! Em que posso te ajudar hoje?"]],
    [r"(qual seu nome\??)", ["Meu nome é ELIZA Clone. Prazer!", "Sou apenas um bot humilde, sem nome bonito."]],
    [r"(adeus|tchau)", ["Tchau! Foi bom conversar com você.", "Até mais!"]],
    [r"(.*)", ["Por que você diz '%1'?"]]
]

chatbot = Chat(pairs, reflections)

if __name__ == "__main__":
    print("Bem-vindo ao ELIZA Clone! (pressione Ctrl+C para sair)")
    chatbot.converse()



Arquivo: classificador_simples.py

from sklearn.feature_extraction.text import CountVectorizer
from sklearn.naive_bayes import MultinomialNB
from sklearn.pipeline import make_pipeline

dados = [
    "Diagnóstico de câncer por imagem",
    "Plataforma de ensino com aprendizado adaptativo",
    "Sistema automatizado de produção industrial",
    "Chatbot para atendimento ao cliente",
    "Análise preditiva para mercado financeiro"
]

categorias = ["Saúde", "Educação", "Indústria", "Serviços", "Finanças"]

modelo = make_pipeline(CountVectorizer(), MultinomialNB())
modelo.fit(dados, categorias)

amostra = ["Reconhecimento de imagem para diagnóstico médico"]
print("Categoria prevista:", modelo.predict(amostra)[0])




3. Visão Estratégica de Gestão de TI (em construção)

Metodologia estruturada baseada no TCC (definição do problema, coleta de dados, modelo, monitoramento)

Roadmap de implementação de IA em ambientes corporativos

Discussões sobre ética, viés algorítmico, privacidade e impactos sociais


Arquivos planejados:

documentacao_estrategica/metodologia_IA_gestao.pdf

roadmap_TI_IA.md

desafios_eticos.md



---

Sobre o Autor

Wallace Antunes Souza é Engenheiro de Software em formação, com MBA em Gestão de Tecnologia da Informação. Apaixonado por IA e transformação digital, busca aplicar tecnologia com propósito e impacto real.

> "A IA não é só tecnologia, é decisão estratégica."






Licença: MIT

Contato: linkedin.com/in/seu-perfil 


