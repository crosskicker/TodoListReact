# React + Vite

<h1>Initialisation</h1>

<h2> Installer d'abord npm</h2>
<b> curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash - </b>
<b> sudo apt-get install -y nodejs </b>
<b> npm create vite@latest projet1 -- --template=javascript -- --jsx=swc </b>
(si tu es pas sous linux c'est pas mon probleme)

<h2>Ensuite git clone mon repo</h2>
<b> git clone https://github.com/crosskicker/TodoListReact.git </b>
This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
