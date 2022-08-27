# Typescript project

## Typescript files

```sh
node tsfile.ts
```

## Typescript projects

*Typescript express*

**File structure**

```
- project
    - src
        - index.ts
    - dist
        - index.js
    - package.json
    - tsconfig.json
    - .env.development
```

**Scripts**

```json
{
    "scripts" : {
        "start": "node dist",
        "build": "tsc",
        "dev": "nodemon -x 'ts-node --log-error' -e ts -r dotenv/config src/index.ts dotenv_config_path=.env.development"
    }
}
```

**tsconfig**

```json
{
    "ts-node": {
        "swc": true,
        "transpileOnly": true
    }
}
```
