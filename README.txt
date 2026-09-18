# cetsp_results

# Fazer um README.txt seguindo o que foi feito para o cvrpn_results


1. Fazer antes de tudo (caso tenha feito mexidas na versão web)
git pull

git add -A
git commit -m "descreva o que voce mudou"
git push


for f in *.mp; do
    mpost "$f"
    epstopdf "${f%.mp}.mps" "${f%.mp}.pdf"
done

rm -f *.mps *.log *.mpx
