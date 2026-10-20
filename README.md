# PARTE 8 — Full Stack Open

React Router para navegación.

## Estructura

```
PARTE8/
└── src_router/
    └── App.jsx              # Componente con BrowserRouter, Route y Link
├── package.json
└── README.md
```

## React Router

El componente `App` usa:

- `BrowserRouter as Router`: Proporciona el contexto de routing
- `Link`: Enlaces navegables sin recargar página
- `Route`: Define la relación entre URL y componente

### Rutas definidas

| Ruta | Componente |
|------|------------|
| `/` | Home |
| `/about` | About |
| `/contact` | Contact |

### Uso

```jsx
<nav>
  <Link to="/">Home</Link> | <Link to="/about">About</Link>
</nav>

<Route exact path="/" component={Home} />
<Route path="/about" component={About} />
```

## Referencia oficial

https://fullstackopen.com/es/part8/router