# React + Vite

<h1>Initialisation</h1>
</br>
</br>
<h2> Installer d'abord npm</h2>
</br>
<b> curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash - </b>
</br>
<b> sudo apt-get install -y nodejs </b>
</br>
<b> npm create vite@latest projet1 -- --template=javascript -- --jsx=swc </b>
</br>
(si tu es pas sous linux c'est pas mon probleme)
</br>
</br>
<h2>Ensuite git clone mon repo</h2>
</br>
<b> git clone https://github.com/crosskicker/TodoListReact.git </b>
</br>
<b> npm run dev </b>
</br>
This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
