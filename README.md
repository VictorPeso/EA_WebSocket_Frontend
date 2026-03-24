# Modificaciones del codigo original

Se ha preparado un video donde se explican y listan todas las modificaciónes realizadas para cumplir con el objetivo buscado. Puedes verlo en YouTube:

[![Video explicativo del proyecto](https://img.youtube.com/vi/R_MzL4CTdQc/0.jpg)](https://youtu.be/R_MzL4CTdQc)

Puedes encontrar el backtend en: https://github.com/VictorPeso/EA_WebSocket_Backend.git

## IA Generativa:

Con el fin de entender al máximo el funcionamiento de WebSocket he priorizado usar el minimo de IA Generativa posible. Limitando su uso a los tres casos contretos:

1. **Autocompletado [GitHub Copilot]**: Uso del autocompletado de Visual Studio Code con el fin de escribir mas rápido o para saber bien bien como se introduce ciertos formatos de datos (p.e. el enum
   dentro del modelo).
2. **Lectura de logs [ChatGPT]**: Explicaciones más detalladas y claras sobre algunos log de errores obtenidos.
3. **Soporte para HTML y CSS [ChatGPT]**: Como son dos lenguajes con los que estoy menos familiarizado he solicitado la creacion de su bloque para usarlo de modelo.

El uso de IA ha sido evitado para cualquier otra situación.

## Preguntes de reflexió

Què passaria si un mateix usuari obre el xat en dues pestanyes diferents? Com podríem evitar que el seu nom surti duplicat?

> Com ja s'explica el video, el que es fa es posar un filtre al service que s'encarrega, avans de fer el push a l'array d'usuaris, comprobar si existeix a la llista, y en cas afirmatiu, és a dir, que
> existeixi, es retorna un error per informar que aquesta acció no es pot dur a terme. Aquesta funcionalitat està implementada y es pot observar a l'arxiu `service/Mensaje.ts`

Per què és millor que el servidor enviï la llista sencera cada vegada en lloc d'enviar només "usuari X s'ha connectat"?

> Perque en cas que hi hagin desconnexions o problemes, el servidor sempre sabra y enviarà la cuantitat exacte d'usuaris dels que te constancia. Si hagués algun problema o error en algun moment no es
> podria saber.

---

# ChatApp

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 21.2.1.

## Development server

To start a local development server, run:

```bash
ng serve
```

Once the server is running, open your browser and navigate to `http://localhost:4200/`. The application will automatically reload whenever you modify any of the source files.

## Code scaffolding

Angular CLI includes powerful code scaffolding tools. To generate a new component, run:

```bash
ng generate component component-name
```

For a complete list of available schematics (such as `components`, `directives`, or `pipes`), run:

```bash
ng generate --help
```

## Building

To build the project run:

```bash
ng build
```

This will compile your project and store the build artifacts in the `dist/` directory. By default, the production build optimizes your application for performance and speed.

## Running unit tests

To execute unit tests with the [Vitest](https://vitest.dev/) test runner, use the following command:

```bash
ng test
```

## Running end-to-end tests

For end-to-end (e2e) testing, run:

```bash
ng e2e
```

Angular CLI does not come with an end-to-end testing framework by default. You can choose one that suits your needs.

## Additional Resources

For more information on using the Angular CLI, including detailed command references, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.
# EA_Sem7_Socket
# EA_Sem7_Socket
