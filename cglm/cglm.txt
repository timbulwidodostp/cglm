# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Causal generalized linear model Use cglm (causalreg) With (In) R Software
install.packages("causalreg")
library("causalreg")
# Estimate Causal generalized linear model Use cglm (causalreg) With (In) R Software
cglm_data = read.csv("https://raw.githubusercontent.com/timbulwidodostp/cglm/main/cglm/cglm.csv",sep = ";")
cglm <- cglm(Y ~ X1 + X2, "poisson", cglm_data, pval = "chi-square", search = "all")
cglm_ <- cglm(Y_ ~ X1 + X2, "binomial", cglm_data, pval = "bootstrap", search = "all")
cglm
cglm_
# Causal generalized linear model Use cglm (causalreg) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished