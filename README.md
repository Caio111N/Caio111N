# Caio Nicollas

**`Desenvolvedora FullStack`**

Me chamo Caio Nicollas, tenho 20 anos e sou de Ribeirão Preto. Estou cursando Ciência da Computação e, paralelamente, me especializando em inglês e desenvolvimento com C#. Tenho interesse em tecnologia, programação e soluções inovadoras, e estou em constante busca por aprendizado prático e desafios que impulsionem minha carreira na área de desenvolvimento de software.
Linkedln: www.linkedin.com/in/caio-nicollas-cunha-reges-1594ab225


---

### 🤖 Linguagens e Tecnologias

<img 
    align="left" 
    alt="HTML"
    title="HTML" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" 
/>
<img 
    align="left" 
    alt="CSS" 
    title="CSS"
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
    alt="C#" 
    title="C#" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/csharp/csharp-original.svg" 
/>
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
    alt="Node.js" 
    title="Node.js" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" 
/>

<img 
    align="left" 
    alt=".NET" 
    title=".NET" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/dot-net/dot-net-original.svg" 
/>




<br/>
<br/>

### 📊 Estatísticas
import os
from collections import defaultdict

# Extensões comuns e suas linguagens
EXTENSOES = {
    '.py': 'Python',
    '.js': 'JavaScript',
    '.ts': 'TypeScript',
    '.java': 'Java',
    '.cpp': 'C++',
    '.c': 'C',
    '.cs': 'C#',
    '.rb': 'Ruby',
    '.go': 'Go',
    '.php': 'PHP',
    '.html': 'HTML',
    '.css': 'CSS',
    '.swift': 'Swift',
    '.rs': 'Rust',
    '.kt': 'Kotlin'
}

def contar_linguagens(diretorio='.'):
    contagem = defaultdict(int)
    for raiz, _, arquivos in os.walk(diretorio):
        for arquivo in arquivos:
            _, ext = os.path.splitext(arquivo)
            linguagem = EXTENSOES.get(ext)
            if linguagem:
                contagem[linguagem] += 1
    return contagem

if __name__ == '__main__':
    estatisticas = contar_linguagens()
    print("📊 Estatísticas de Linguagens no Repositório:")
    for linguagem, quantidade in sorted(estatisticas.items(), key=lambda x: -x[1]):
        print(f"{linguagem}: {quantidade} arquivos")


