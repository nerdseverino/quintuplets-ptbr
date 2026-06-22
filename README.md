# 🇧🇷 Tradução PT-BR — The Quintessential Quintuplets: Five Memories Spent With You

Tradução para Português do Brasil da visual novel **The Quintessential Quintuplets: Five Memories Spent With You** (5等分の花嫁 ~君と過ごした五つの思い出~).

> ⚠️ **Tradução automática** — Feita via Google Translate. Contribuições para melhorar a qualidade são muito bem-vindas!

## 📊 O que foi traduzido

| Conteúdo | Quantidade |
|----------|------------|
| Diálogos (cenários) | ~29.000 linhas (360 cenários) |
| Interface (menus, botões, mensagens) | 148 textos |
| Conquistas | 26 conquistas |

## 📥 Qual versão baixar?

| Sua versão do jogo | Release para baixar |
|---------------------|---------------------|
| **Steam** (comprado na loja) | [v2.0 - Steam Oficial](../../releases/tag/v2.0) |
| **SteamRIP / Tenoke** (crack) | [steamrip](../../releases/tag/steamrip) |

> Não sabe qual é a sua? Se você comprou o jogo na Steam, use a v2.0. Se baixou de outro lugar, use a steamrip.

---

## 🪟 Instalação no Windows

### Passo a passo

1. **Baixe** a release correta para sua versão (veja tabela acima)
2. **Localize a pasta do jogo:**
   - Steam: clique com botão direito no jogo na Biblioteca > Gerenciar > Navegar em Arquivos Locais
   - SteamRIP: a pasta onde você extraiu o jogo
3. **Faça um backup** (copie a pasta `windata` para outro lugar, caso queira reverter depois)
4. **Copie os arquivos traduzidos:**
   - Copie `windata/scenario_body.bin` para a pasta `windata/` do jogo (substituindo o original)
   - Copie `windata/config_body.bin` para a pasta `windata/` do jogo (substituindo o original)
5. **Configure o idioma:** abra o jogo e selecione **English** no menu de idiomas

Pronto! O texto vai aparecer em português.

### Por que selecionar "English"?

A tradução substitui o texto inglês por português. Não é criado um idioma novo no menu. Ao selecionar English, o jogo carrega o texto que agora está em pt-BR.

---

## 🐧 Instalação no Linux / Steam Deck

### Método rápido (script)

```bash
git clone https://github.com/nerdseverino/quintuplets-ptbr.git
cd quintuplets-ptbr
chmod +x instalar.sh
./instalar.sh "/caminho/para/pasta/do/jogo"
```

O script detecta a pasta do jogo automaticamente se você estiver dentro dela, ou você pode passar o caminho como argumento.

**Caminho padrão da Steam no Deck:**
```
~/.local/share/Steam/steamapps/common/goto02
```

### Método manual

1. Baixe a release v2.0
2. Copie os arquivos para a pasta `windata/` do jogo:
```bash
cp windata/scenario_body.bin ~/.local/share/Steam/steamapps/common/goto02/windata/
cp windata/config_body.bin ~/.local/share/Steam/steamapps/common/goto02/windata/
```
3. No jogo, selecione idioma **English**

---

## ↩️ Como reverter (desinstalar a tradução)

### Se usou o script de instalação
O script cria backups automáticos com extensão `.bkp-TIMESTAMP`. Para reverter:
```bash
cd /caminho/para/pasta/do/jogo/windata
mv scenario_body.bin.bkp-* scenario_body.bin
mv config_body.bin.bkp-* config_body.bin
```

### Se copiou manualmente
Restaure os arquivos da pasta `windata` que você copiou como backup antes de instalar.

### Alternativa (Steam)
Use a opção "Verificar integridade dos arquivos do jogo" nas propriedades do jogo na Steam. Isso vai restaurar os arquivos originais.

---

## 🤝 Como Contribuir

A tradução automática tem limitações. Nomes de personagens, expressões idiomáticas e contexto emocional podem estar incorretos.

### Reportar erros
Abra uma [Issue](../../issues) com:
- Captura de tela do texto incorreto
- Cenário/capítulo onde aparece (se possível)
- Sugestão de tradução correta

### Contribuir com correções
1. Fork este repositório
2. Edite `translation_cache.json` (formato: `"texto em inglês": "texto em português"`)
3. Abra um Pull Request

### Prioridades de revisão
- [ ] Nomes próprios (personagens, lugares)
- [ ] Expressões idiomáticas traduzidas literalmente
- [ ] Contexto de falas românticas/emocionais
- [ ] Legendas de vídeo (cutscenes)

---

## 🔧 Detalhes Técnicos

- Engine: M2/EMote (arquivos PSB)
- Ferramentas: [FreeMote](https://github.com/UlyssesWu/FreeMote), [deep-translator](https://github.com/nidhaloff/deep-translator)
- Método: substituição direta na string table dos PSBs
- Fontes do jogo já suportam caracteres acentuados (NotoSans)

## 📜 Créditos

- Tradução: Google Translate via deep-translator
- Extração/empacotamento: FreeMote por UlyssesWu
- Manutenção: [@nerdseverino](https://github.com/nerdseverino)
