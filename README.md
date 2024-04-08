# React + Vite

(avoir node de deja installé -> node -v)

curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
sudo apt-get install -y nodejs

npm create vite@latest projet1 -- --template=javascript -- --jsx=swc

<b> Initialisation </b>

npm create vite@latest projet1 -- --template react-swc

cd projet1

git clone https://

npm install

npm install -D sass

<b> Lancement  </b>

npm run dev 

http://localhost:5173



This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
