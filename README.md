# Kudondza Center

**Centro de Aprendizagem, Tecnologia e Desenvolvimento**

_Aprender. Criar. Desenvolver._

Este repositório reúne o trabalho do Kudondza Center: programas dos cursos, preparação das aulas, materiais para os estudantes, divulgação e o site.

## Cursos

| Curso | Estado | Pasta |
|---|---|---|
| Informática Básica e Competências Digitais | Inscrições abertas | [`cursos/informatica-basica`](cursos/informatica-basica/) |

## Estrutura

```
.
├── .github/workflows/pages.yml  publica o site no GitHub Pages
├── cursos/
│   └── informatica-basica/
│       ├── README.md            ficha do curso: oferta, programa e pontos por definir
│       ├── guia-do-curso.md     guia completo de módulos e conteúdos
│       ├── aulas/               plano de cada aula, com link para os slides
│       └── originais/           documentos recebidos (.docx), guardados como referência
├── divulgacao/
│   └── flyer-informatica-basica.webp
└── site/                        site público (HTML e CSS, sem compilação)
    ├── index.html
    ├── styles.css
    └── img/
```

Site: **<https://duarte-mondlane.github.io/kudondza/>**. É publicado automaticamente a partir do `main`; o [`site/README.md`](site/README.md) explica como.

## Convenções

- O conteúdo editável fica em Markdown (`.md`), para se poder ver e comparar as alterações no histórico.
- Os documentos originais (Word, PDF, imagens) ficam numa pasta `originais/` junto do conteúdo a que dizem respeito.
- Nomes de ficheiros e pastas em minúsculas, sem acentos, com hífens: `plano-aula-01.md`.

## Contactos

- Telefone: +258 87 999 4892
- E-mail: kudonzacenter@gmail.com
