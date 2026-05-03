# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Bias Diagnostic for Linear Mixed Models Use mixedbiastest With (In) R Software
install.packages("mixedbiastest")
install.packages("plm")
library("mixedbiastest")
library("plm")
library("lme4")
# Estimation Bias Diagnostic for Linear Mixed Models Use mixedbiastest With (In) R Software
mixedbiastest = read.csv("https://raw.githubusercontent.com/timbulwidodostp/mixedbiastest/main/mixedbiastest/mixedbiastest.csv",sep = ";")
mixedbiastest <- lmer(mixedbiastest ~ mixedbiastest_1 + mixedbiastest_2 + mixedbiastest_3 + (1 | country), data = mixedbiastest)
mixedbiastest <- mixedbiastest(mixedbiastest)
print(mixedbiastest); plot(mixedbiastest)
# Bias Diagnostic for Linear Mixed Models Use mixedbiastest With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished