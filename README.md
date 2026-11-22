# Amic invisible

Pàgina estàtica per repartir els sobres d'un amic invisible sense que ningú —
ni tan sols qui organitza el sorteig — sàpiga a qui li ha tocat cadascú.

## Com funciona

L'assignació no es desa enlloc: viatja **dins del codi**, al fragment de l'URL.

```
https://<usuari>.github.io/amic-invisible/#87NT-99W6-YM
                                           └─ nom propi i nom de qui rep, xifrats
```

El fragment (`#…`) no s'envia mai al servidor: el navegador el reté i la pàgina el
descodifica en local. Per això aquest repositori **no conté cap assignació** i el
servidor no en pot registrar cap.

Si l'enllaç falla, la mateixa pàgina demana el codi escrit a mà. Accepta
minúscules, espais i guions indistintament, i corregeix les confusions típiques
(`O` per `0`, `I` i `L` per `1`, `U` per `V`). Un codi mal escrit es rebutja gràcies
a una suma de control; no obre mai un sobre equivocat.

## Tres maneres d'obrir el sobre

| Via | Per a qui |
| --- | --- |
| Tocar l'enllaç rebut per WhatsApp | Sèniors i qualsevol amb mòbil |
| Escanejar un codi QR | Infants amb iPad o ordinador, sense mòbil |
| Escriure el codi a mà | Rescat si l'enllaç no s'obre |

## Condicions del sorteig

El repartiment es genera fora d'aquesta pàgina i compleix:

- Ningú es regala a ell mateix.
- Cada sènior rep el regal d'un infant.
- Cap intercanvi directe: si A regala a B, B no regala a A.
- Un sol regal rebut i un sol regal fet per persona.

## Abast real de la protecció

El codi evita que l'assignació es pugui llegir a ull i que un error de
transcripció obri el sobre d'algú altre. No és criptografia: qui tingui l'enllaç
o el codi d'una altra persona en veurà el contingut, i no queda cap rastre. La
llista completa de codis es guarda a part i no es publica mai aquí.
