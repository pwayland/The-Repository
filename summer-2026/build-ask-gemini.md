Tengo *antigravity CLI* instalado y accesible con comando `Gemini`. Ayúdame a diseñar una herramienta para que Codex utilice Gemini.

## Nombre

Quiero utilizar `ask-gemini` como *comando* para que llames a la herramienta.

## Usuario

El usuario soy yo, desde Codex. Quiero que algunos proyectos puedan *ask-gemini* (y me informen) cuando piensen añada utilidad aunque yo no la haya solicitado.

## Problema

El modelo produce resultados consistentes (similares). Ejercicios de *segunda opinión* o *evaluación adversarial* con un segundo modelo deberían funcionar mejor.

## Trigger

`ask-gemini` es indicador de que debes llamar a la herramienta. También debes llamar la herramienta cuando pienses que vaya a añadir valor.

## Inputs

Codex escribirá el prompt para obtener información útil de Gemini, escogerá que archivos podrá acceder y si debe buscar en internet; a base del contexto y mis instrucciones.

## Tools needed

- web search
- read access to specific files on occasion

## lentes

En algunos casos necesito que añadas instrucciones para un tipo de *mirada* en lugar o adicional a la *general*. Lentes:
- **nombre | intención**
- adversary | Deliver critical, logical opposition with direct intensity to expose weaknesses and strengthen ideas through rigorous stress-testing
- architect | Communicate with unwavering coherence and honesty through reflective, reality-grounded discourse that resists flattery and maintains integrity across multiple levels of meaning
- provocador | Challenge conventional wisdom through provocative, playful exploration of unconventional ideas and radical combinations
- realist | Deliver precise, analytical insights with candid directness, prioritizing clarity and substantive depth over pleasantries


## Codex decide

El modelo (AI, Codex) deben invocar *ask-gemini* cuando entienda añada valor. Cuando Codex llama a Gemini sin instrucción previa debe escoger lente, si alguno, e informar que utilizó herramienta.
Cuando reciba instrucción de *ask-gemini* sin especificar lente, puede escoger alguno si entiende es apropiado.

## Humano decide
Yo puedo llamar la herramienta en cualquier momento y escoger lente que quiera. Cualquier paso que incorporé *ask-gemini* debe terminar en un plan; NO en editar archivos.

## Approval points

Necesitas aprobación para ejecutar cualquier plan luego de consultar a Gemini.

## Log/audit trail

Mantén un historial de consultas con Gemini

## crea un plan / pide aprobación

Haz un plan antes de ejecutarlo. Pídeme aprobación para poderlo revisar.
