# admiss-o-
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Formulário de Admissão</title>
  <style>
    body { font-family: Arial; padding: 20px; background-color: #f4f4f4; }
    form { max-width: 500px; margin: auto; background: white; padding: 20px; border-radius: 8px; }
    label { display: block; margin-top: 10px; }
    input, textarea { width: 100%; padding: 8px; margin-top: 5px; }
    button { margin-top: 20px; padding: 10px; width: 100%; background-color: #007bff; color: white; border: none; border-radius: 4px; }
  </style>
</head>
<body>
  <h2 style="text-align: center;">Formulário de Admissão</h2>
  <form id="admissaoForm">
    <label>Nome completo:</label>
    <input type="text" name="nome" required />

    <label>E-mail:</label>
    <input type="email" name="email" required />

    <label>Telefone:</label>
    <input type="tel" name="telefone" required />

    <label>Endereço:</label>
    <input type="text" name="endereco" required />

    <label>Data de nascimento:</label>
    <input type="date" name="nascimento" required />

    <label>Foto (perfil):</label>
    <input type="file" name="foto" accept="image/*" required />

    <label>Link do GitHub:</label>
    <input type="url" name="github" placeholder="https://github.com/seuperfil" />

    <label>Experiências:</label>
    <textarea name="experiencias" rows="5" placeholder="Conte suas experiências profissionais..."></textarea>

    <button type="submit">Enviar</button>
  </form>

  <script>
    const form = document.getElementById('admissaoForm');
    form.addEventListener('submit', function(event) {
      event.preventDefault();
      alert('Formulário enviado! (mas ainda não está salvando em lugar nenhum)');
    });
  </script>
</body>
</html>
