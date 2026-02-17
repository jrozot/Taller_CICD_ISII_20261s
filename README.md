# Taller 1 CI/CD Ing. de Software II un
**Estudiante:** Juan Mateo Rozo Torres
Se ha desarrollado el taller de acuerdo al enunciado en /docs/taller_cicd.pdf

## Capturas de pantalla:
- **Pipeline funcional:**

- **Pruebas en Github Actions:**

- **Despliegue en Github Pages:**


## Solución del ejercicio endpoint GET:
- Se ha agregado el siguiente código a /src/app.js
```js
app.get('/version', (req, res) => {
  res.json({ version: '1.0.0' });
});
```
- Se ha agregado el siguiente test.
```js
test('GET /version should return version 1.0.0', async () => {
  const response = await request(app).get('/version');
  expect(response.status).toBe(200);
  expect(response.body.version).toBe('1.0.0');
});
```
- **Captura de pantalla:**
