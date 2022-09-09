# ![DevSuperior logo](https://raw.githubusercontent.com/devsuperior/bds-assets/main/ds/devsuperior-logo-small.png) Semana Spring React - Episódio 3
>  *Crie um app completo para seu portfólio com as tecnologias mais demandadas do mercado*

## Realização
[DevSuperior - Escola de programação](https://devsuperior.com.br)

[![DevSuperior no Instagram](https://raw.githubusercontent.com/devsuperior/bds-assets/main/ds/ig-icon.png)](https://instagram.com/devsuperior.ig)
[![DevSuperior no Youtube](https://raw.githubusercontent.com/devsuperior/bds-assets/main/ds/yt-icon.png)](https://youtube.com/devsuperior)

## Objetivos do projeto para esta aula
- Integrar back end e front end
- Implantar o front end

## AVISO: as aulas ficarão disponíveis somente até domingo às 23h59

# Checklist

## Passo: Primeira requisição com Axios e useEffect

```
yarn add axios@0.27.2
```

- **COMMIT: Axios, useEffect first request**

## Passo: Listagem de vendas

Definição da BASE_URL:

```javascript
export const BASE_URL = import.meta.env.VITE_BACKEND_URL ?? "http://localhost:8080";
```

- **COMMIT: Sale listing**

## Passo: Passando as datas como argumento

- **COMMIT: Date update**

## Passo: Enviar notificação

- **COMMIT: Send notification**

## Passo: Mensagem Toast de confirmação

```
yarn add react-toastify@9.0.5
```

No App.tsx:
```javascript
import { ToastContainer } from 'react-toastify';
import 'react-toastify/dist/ReactToastify.css';
```

- **COMMIT: Toast**

## Passo: Deploy no Netlify

Antes: acrescente `window.React = React` no seu main.tsx conforme abaixo, e salve um novo commit:

```js
import React from 'react'
import ReactDOM from 'react-dom/client'
import App from './App'
import './index.css'

window.React = React

ReactDOM.createRoot(document.getElementById('root') as HTMLElement).render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
)
```

https://www.netlify.com/

- Deploy básico
  - Base directory: frontend
  - Build command: yarn build
  - Publish directory: frontend/dist
  - Variáveis de ambiente:
    - VITE_BACKEND_URL

- Configurações adicionais
  - Site settings -> Domain Management: (colocar o nome que você quiser)
  - Deploys -> Trigger deploy


## PARABÉNS!

![Parabéns!](https://raw.githubusercontent.com/devsuperior/bds-assets/main/img/trophy.png)

- Quero muito saber seu feedback
  - O que você está achando da nossa abordagem?
  - Você está conseguindo acompanhar?
  - O que você está achando do evento?
- Participe
  - Comente no Instagram e marque a gente @devsuperior.ig
  - Divulgue seu projeto no Linkedin e marque a DevSuperior
