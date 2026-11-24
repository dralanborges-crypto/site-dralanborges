# Guia de publicação do site

Como colocar o site no ar. São arquivos estáticos — HTML e uma folha de estilo, sem banco de dados e sem programação. Funciona em qualquer hospedagem.

---

## Arquivos

```
index.html                 → página inicial (osteopata em Londrina)
osteopatia.html            → o que é osteopatia
dor-lombar.html            → dor lombar
dor-cervical.html          → dor cervical
ciatica.html               → ciática
osteopatia-pediatrica.html → bebês e crianças
enxaqueca-dtm.html         → enxaqueca e DTM
metodo-sib.html            → Método SIB
cursos.html                → cursos e formação
estilo.css                 → folha de estilo única (comum a todas as páginas)
favicon.ico / .svg / .png  → ícone da aba e do atalho no celular
manifest.json              → configuração do ícone em dispositivos
img/                       → fotos do site (hero e compartilhamento)
```

Os arquivos devem ficar **todos na mesma pasta**, sem subpastas.

---

## Passo 1 — Domínio

`dralanborges.com.br` **já está registrado no seu nome** — verifiquei no Registro.br. O que falta é apontar o DNS para a hospedagem (o domínio existe, mas hoje não responde).

- Confirme o acesso à conta do Registro.br (registro.br) — o domínio já é seu; você vai precisar entrar lá só para apontar os servidores DNS.
- Precisa de CNPJ ou CPF e de um e-mail para contato.

**Alternativa gratuita, se quiser começar hoje:** publicar no endereço que já existe. Hoje, `sibonline.dralanborges.com.br` é uma aplicação JS que o Google lê como uma frase só. Trocando os arquivos, o site já funciona — mas atenção: isso substitui a aplicação atual, então confirme com quem cuida dela.

---

## Passo 2 — Hospedagem

Opções, da mais simples à mais completa:

| Opção | Custo | Observação |
|---|---|---|
| **Netlify** (netlify.com) | grátis | Arraste a pasta no painel e o site sobe. Ideal para começar. |
| **Cloudflare Pages** | grátis | Rápido no Brasil, bom para SEO. |
| **Hostinger / KingHost** | ~R$ 10–25/mês | Hospedagem brasileira, suporte em português. |

### Se for Netlify (caminho mais rápido)

1. Crie a conta em netlify.com (pode entrar com Google).
2. Clique em **Add new site → Deploy manually**.
3. Arraste a pasta `site` inteira para a área indicada.
4. O site já está no ar em um endereço `nome-aleatorio.netlify.app`.
5. Em **Domain settings → Add custom domain**, digite `dralanborges.com.br` e siga as instruções de DNS que o Netlify mostrar (aponta o domínio do Registro.br para o Netlify).

### Se for hospedagem tradicional (Hostinger, KingHost)

1. Contrate o plano e pegue os dados de acesso (FTP ou painel hPanel).
2. Abra o **Gerenciador de Arquivos** do painel.
3. Entre na pasta `public_html`.
4. Envie os 8 arquivos para dentro dela — **não** envie a pasta, envie os arquivos.
5. Aponte o domínio para a hospedagem no Registro.br (servidores DNS que a hospedagem informar).

---

## Passo 3 — Depois de publicar

- [ ] Abra o site no celular e no computador e confira todas as páginas
- [ ] Teste o botão de WhatsApp: ele deve abrir a conversa com uma mensagem já escrita
- [ ] Teste o botão de ligar em um celular
- [ ] Cadastre o site no **Google Search Console** (search.google.com/search-console) — adicione a propriedade e envie o sitemap
- [ ] Atualize o link do Perfil da Empresa no Google para o site novo
- [ ] Atualize o link da bio do Instagram
- [ ] Cadastre no Bing Places (bingplaces.com)

## Sobre o sitemap

O arquivo `sitemap.xml` já está incluído, apontando para `dralanborges.com.br`. Se você publicar em outro domínio, é preciso trocar o endereço dentro dele (é um arquivo de texto, basta editar).

---

## O que ainda falta e precisa de você

- **Fotos.** A foto principal foi aplicada no hero da home: `img/dr-alan-borges.jpg` (900×1200) e `img/dr-alan-borges-540.jpg` (versão mobile), mais `img/og-dralanborges.jpg` (1200×630) para compartilhamento em redes e WhatsApp. Escolhida entre 4 opções enviadas pelo Alan. Faltam ainda imagens internas (fachada, sala de atendimento, consultório) para as páginas de serviço.
- **Logo.** Hoje o cabeçalho é tipográfico (o nome escrito). Se você tem a marca em arquivo, me manda que eu aplico.
- **Endereço.** **Av. Madre Leônia Milito, 1500 — sala 409, Atsushi Yoshii Tower, Gleba Palhano, Londrina · PR, 86050-270** — endereço do Instituto Alan Borges, usado em todas as páginas do site.
- **Valores de consulta**, se quiser publicar (não é obrigatório; muitas clínicas preferem o contato).
