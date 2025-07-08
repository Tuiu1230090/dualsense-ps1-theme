/* Fundo retrô PS1 */
body {
    background: #c0c0c0 !important;
}

/* Filtro retrô na carcaça do controle */
#controller {
    filter: contrast(1.1) brightness(1.05) grayscale(0.4);
}

/* Ajuste nos botões principais - usando filtros de cor */
img[src*="button-south"] {
    filter: hue-rotate(210deg) saturate(2); /* X azul */
}
img[src*="button-east"] {
    filter: hue-rotate(330deg) saturate(2); /* O vermelho */
}
img[src*="button-west"] {
    filter: hue-rotate(290deg) saturate(2); /* quadrado rosa */
}
img[src*="button-north"] {
    filter: hue-rotate(100deg) saturate(2); /* triângulo verde */
}

/* Botão PS central (levemente mais escuro) */
img[src*="button-meta"] {
    filter: grayscale(1) brightness(0.7);
}

/* Ombros L1/R1 e L2/R2 com contraste retrô */
img[src*="shoulder"], img[src*="trigger"] {
    filter: grayscale(1) brightness(0.85);
}

/* Direcional e botões Start/Select levemente desbotados */
img[src*="dpad"], img[src*="start"], img[src*="select"] {
    filter: grayscale(0.5) brightness(0.9);
}
