# Du-Lite
## Projeto em C de implementação simples do comando du

Programa é chamado: `$ ./du-lite <ditretorio-alvo> <N>`

Exemplo: `$ ./du-lite /home/pedro 10` -> Acha os 10 maiores gastadores de espaço em /home/pedro/

Programa não faz a recursão em pastas, exemplo para o alvo /home/pedro, projeto dá o tamanho total da pasta /home/pedro/MEGA, mas não dá o tamanho das subpastas dentro de MEGA, apenas as contabiliza para totalizar MEGA
#
Projeto usa as bibliotecas:
* `libfileutils` -> https://github.com/PedroF37/FileUtils
* `libdirutils` -> https://github.com/PedroF37/DirUtils
#
Projeto é compilado com: `$ clang -Wall -Wextra --pedantic -std=c99 -ldirutils -lfileutils -o du-lite du-lite.c`
