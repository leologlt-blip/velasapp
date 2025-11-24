VelasApp - Projeto Android (Kotlin, Jetpack Compose, Room) - Versão Completa
---------------------------------------------------------------------------

Novidades nesta versão:
- Clientes: CPF, WhatsApp, endereço, observações, data de cadastro, fotoUri (campo texto)
- Produtos: SKU, categoria, custo, preço, estoque, alerta de estoque, fotoUri (campo texto)
- Vendas: formaPagamento, desconto, total calculado automaticamente, compartilhar por WhatsApp
- Entradas de estoque: registrar compra que aumenta o estoque
- Backup: exportar banco para JSON (arquivo em cache)
- Export: exportar vendas para CSV e enviar por apps (compartilhar)
- PIN simples na entrada (padrão 1234)
- Indicação visual quando estoque baixo (cartão com fundo claro)
- Tema escuro disponível no código (ajuste futuro)
- Arquitetura baseada em Room e Compose (simples de estender)

Como abrir e gerar APK (passo-a-passo):
1) Baixe e instale o Android Studio (recomendo Flamingo ou mais recente).
2) Extraia este zip e abra a pasta 'VelasApp_full' no Android Studio (Open an existing project).
3) Deixe o Gradle sincronizar. Se o Android Studio pedir atualização de plugins/kotlin, aceite e sincronize novamente.
4) Conecte um dispositivo Android (USB debugging) ou use um emulador.
5) Build -> Build Bundle(s) / APK(s) -> Build APK(s). Após o build, escolha 'Locate' para achar o APK.
6) Para permitir export/import via FileProvider, adicione provider no AndroidManifest se necessário (exemplo próximo versão).
7) Assine o app para publicar (opcional). Para instalar localmente, você pode usar o APK gerado.

Observações importantes:
- Fotos não são capturadas automaticamente: os campos fotoUri aceitam URIs (próxima versão vai incluir picker de imagens).
- Import automático do backup é placeholder; eu posso implementar import automático numa versão a seguir.
- Compartilhar CSV usa FileProvider; Android Studio pode solicitar ajustes no manifest - eu posso ajustar conforme seu dispositivo.

Próximos que eu posso fazer pra ti (escolhe um):
- Implementar picker de imagens para clientes/produtos e salvar URI localmente
- Gerar recibo em PDF automaticamente
- Integrar envio automático de venda por WhatsApp com botão direto para número do cliente
- Implementar import JSON completo para restaurar banco
- Ajustes visuais (ícones, cores, logo com sua vela/branding)
- Build e envio do APK pronto (posso gerar se tu me der confirmação para criar o APK aqui)

Boa! - Chat (GPT)
