# Bonfire Desktop

Instaladores do app desktop do **Bonfire**, que faz backups automáticos (restic) das pastas do seu computador para o seu Umbrel.

Este repositório só guarda os instaladores. Baixe a versão mais recente em **[Releases](../../releases/latest)**.

## Qual arquivo baixar

| Sistema | Arquivo |
|---|---|
| Windows (x64) | `Bonfire_<versão>_x64-setup.exe` (ou `.msi`) |
| macOS com Apple Silicon (M1 ou mais novo) | `Bonfire_<versão>_aarch64.dmg` |
| macOS com Intel | `Bonfire_<versão>_x64.dmg` |

## Instalação

Os builds não são assinados, então o sistema avisa na primeira vez que o app é aberto.

**Windows:** abra o instalador. Se aparecer o SmartScreen, clique em **Mais informações › Executar assim mesmo**.

**macOS:** abra o `.dmg` e arraste o Bonfire para **Aplicativos**. Depois rode no Terminal:

```bash
xattr -dr com.apple.quarantine /Applications/Bonfire.app
```

Sem esse comando, o macOS diz que o app "está danificado".

## Primeiro uso

1. Instale o app **Bonfire** no seu Umbrel.
2. No painel do Bonfire no Umbrel, gere um código de pareamento.
3. Abra o app desktop, informe o endereço do Umbrel e o código, e escolha as pastas para o backup.
