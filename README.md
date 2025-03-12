<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Criação de Evento</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-300">

    <header class="bg-black text-white p-5 min-h-[368px] flex flex-col items-center justify-center text-center">
        <h1 class="text-2xl font-bold p-1">Crie e compartilhe seu evento.</h1>
        <p class="text-cyan-300 mt-4">Primeiro, é só preencher esse formulário aqui embaixo.</p>
    </header>

    <div class="bg-white max-w-3xl mx-auto p-6 mt-[-42px] rounded-lg shadow-lg border">
        <form action="#">
            <div class="mb-4">
                <label class="block text-gray-700">Título do evento</label>
                <input type="text" class="w-full border rounded p-2 mt-1" placeholder="Nome do seu evento" required>
            </div>
            
            <div class="mb-4">
                <label class="block text-gray-700">Link do evento</label>
                <input type="url" class="w-full border rounded p-2 mt-1" placeholder="Coloque o https:// aqui" required>
            </div>
            
            <div class="mb-4">
                <label class="block text-gray-700">WhatsApp pra contato</label>
                
                <input type="text" class="w-full border rounded p-2 mt-1 border-red-500" placeholder="Só número, tipo 11987654321" required>
            </div>
            
            <div class="mb-4">
                <label class="block text-gray-700">Detalhes extras</label>
                <textarea class="w-full border rounded p-2 mt-1" placeholder="Algo a mais pra contar?"></textarea>
            </div>
            
            <div class="mb-4">
                <label class="block text-gray-700">Categoria</label>
                <select class="w-full border rounded p-2 mt-1" required>
                    <option value="">Escolhe o tipo de evento</option>
                    <option value="1">Conferência</option>
                    <option value="2">Workshop</option>
                    <option value="3">Seminário</option>
                </select>
            </div>
            <h2 class="text-lg font-semibold text-gray-800 mt-4">Privacidade</h2>
            <div class="mb-4">
                <label class="block text-gray-700">E-mail do organizador</label>
                <input type="email" class="w-full border rounded p-2 mt-1" placeholder="Seu e-mail aqui" required>
            </div>
            
            <div class="mb-4">
                <label class="block text-gray-700">Senha pros participantes</label>
                <input type="password" class="w-full border rounded p-2 mt-1" placeholder="Mínimo 6 letras/números" minlength="6" required>
            </div>
            
            <div class="mb-4">
                <label class="inline-flex items-center">
                    <input type="checkbox" class="text-green-500" checked>
                    <span class="ml-2 text-gray-700">Evento privado (só quem tem senha entra)</span>
                </label>
            </div>
            <h2 class="text-lg font-semibold text-gray-800 mt-4">Dia e hora</h2>
            <div class="flex flex-col md:flex-row gap-4 mb-4">
                <input type="date" class="w-full border rounded p-2 mt-1" required>
                <input type="time" class="w-full border rounded p-2 mt-1" required>
                <input type="time" class="w-full border rounded p-2 mt-1" required>
            </div>
            <button type="submit" class="w-full bg-green-500 text-white font-bold py-2 px-4 rounded hover:bg-green-600">
                Salvar meu evento
            </button>
        </form>
    </div>
</body>
</html>
          
