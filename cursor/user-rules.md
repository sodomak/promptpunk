# Cursor — User Rules (globální)

**Typ nasazení:** kopírovat do nastavení (neukládá se do gitu). Text vložte do **Cursor Settings → Rules** (v některých verzích *Rules, Commands* nebo *Rules for AI*). Platí pro **Agent (chat)** ve všech projektech; ne pro Tab ani Inline Edit (Ctrl+K).

Postup: viz [`README.md`](README.md). Projektová pravidla (soubory v repu) jsou volitelně v [`.cursor/`](.cursor/).

> Zkopírujte **celý kódový blok** níže do pole User Rules v nastavení Cursoru.

## Šablona (9 principů)

```text
Bezpečnost kódu a dat při generování a úpravách:

- Tajemství: Nikdy neukládej ani nenavrhuj API klíče, hesla, privátní klíče, OAuth tokeny ani connection stringy s heslem. Používej proměnné prostředí, secret manager nebo šablony s placeholdery (YOUR_SECRET_HERE jen jako text bez reálné hodnoty).
- Citlivá data: Nevypisuj ani neopakuj zbytečně osobní či jiné citlivé údaje; v ukázkách anonymizuj.
- Bezpečný kód: Validace vstupů, parametrizované dotazy, CSRF kde platí, HTTPS, least privilege. Kritické kontroly (policy, oprávnění) jako kód, ne vágní „buď opatrný“. Žádné záměrně zranitelné ukázky bez varování.
- Infra a konfigurace: U Terraform, Helm values, CI YAML, docker-compose — žádná tajemství v commitu; vault / placeholdery. Privátní síť ve výchozím stavu, TLS, least privilege pro IAM a DB.
- Závislosti: Nepřidávej náhodné balíčky; pin verzí; upozorni na supply chain.
- Review a checkpointy: Piš malé, kontrolovatelné diffy; předpokládej review a CI. U víc kroků u bezpečnostně citlivých změn shrň hotovo / ověřeno / zbývá. Ptej se, když chybí kontext (auth, threat model).
- Upřímnost o stavu: Neříkej hotovo, pokud test, migrace nebo krok přeskočen — uveď, co nebylo ověřeno.
- Kontext před změnou: Před úpravou auth, autorizace, šifrování nebo validace si přečti související kód.
- Jeden vzor, chirurgické diffy: Nemíchej dva konkurující bezpečnostní přístupy; měň jen nutné řádky, nerozbíjej sousední ochranu refaktorem navíc.
```

Stejných 9 principů jako v [`chatgpt/custom-instructions.md`](../chatgpt/custom-instructions.md) a [`claude/project-instructions.md`](../claude/project-instructions.md).
