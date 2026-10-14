# Desafío: de la bandeja al takedown

Material de la charla "De la bandeja al takedown" (Richard Pérez).
Son 4 casos reales. Probá hacer el mismo análisis que vimos en la charla.

## Reglas de seguridad
- NO hagas clic en ningún link de los mails.
- Abrí los .eml con un editor de texto (Bloc de notas, VS Code), no con Outlook.
- Al sitio del caso 4 NO entres: usá solo el informe de urlscan (ya lo visitó por vos).

## Caso 1, 2 y 3 (carpeta casos/)
Tres mails en formato .eml. Para cada uno:
1. Pegá las cabeceras en MXToolbox (Email Header Analyzer) y mirá SPF, DKIM y DMARC.
2. ¿Coincide From, Return-Path y Reply-To? ¿Quién envió realmente el mail?
3. Sacá las URLs. Si hay acortador, verificalo en urlscan.io (nunca abriéndolo vos).
4. Mirá la IP y el dominio en VirusTotal, AbuseIPDB, bgp.he.net y lookup.icann.org.
5. ¿A quién reportarías (hosting, registrar, plataforma)?

## Caso 4: el kit de phishing
Informe de urlscan (público, sitio ya visitado por urlscan):

https://urlscan.io/result/01a13272-dd2a-75c8-8775-08e049aef223/

Preguntas:
1. ¿Qué marca imita? Mirá el screenshot.
2. En la pestaña HTTP: ¿de dónde carga el logo? ¿Qué es ip.js? ¿Qué plataforma lo hospeda?
3. En la pestaña Content / DOM: encontrá el script del formulario. ¿Adónde envía lo que escribe la víctima? (Si ves un token de bot, no lo uses.)
4. ¿A quién reportás y por qué canal? (phish.report te ayuda a encontrar los contactos.)
5. ¿Cómo sabés que el takedown funcionó? (pista: rescan)

## Herramientas
MXToolbox · urlscan.io · VirusTotal · AbuseIPDB · bgp.he.net · lookup.icann.org · phish.report · CyberChef
