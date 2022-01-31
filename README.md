# Economics-Data-Scientist-Intern
Prova para estágio

poctes instalados para fazer exercício.
install.packages("readxl")
library(readxl)
install.packages("dplyr")
library(dplyr)
install.packages("stringr")
library(stringr)


setwd("C://Users//ticob//OneDrive//Documentos//Projeto GitHub//Economics-Data-Scientist-Intern") #acessar a pasta na qual o arquivo estava no computador.
df <- read_excel ("pmc.xlsx", skip = 3) #importar arquivo Excel pulando as 3 linhas iniciais.
colnames(df) <- c("Data", "Var", "setor", "BR", "CE", "PE", "BA", "MG", "ES", "RJ", "SP", "PR", "SC", "RS", "GO", "DF") #Renomear colunas.
df <- df %>% mutate(BR = as.numeric(BR), CE = as.numeric(CE), PE = as.numeric(PE), BA = as.numeric(BA), MG = as.numeric(MG), ES = as.numeric(ES), RJ = as.numeric(RJ), SP = as.numeric(SP), PR = as.numeric(PR), SC = as.numeric(SC), RS = as.numeric(RS), GO = as.numeric(GO), DF = as.numeric(DF)) #Converter colunas específicas e para tipo número.

for (Var in 1:nrow(df)){
df <- str_replace(df[r,2], regex, "Volume")".*(\\bvolume\\b).*"} #alterar nome das linhas para Volume.



dd <- read.csv ("rendimento_efetivo_real.csv", header = TRUE, sep = ";") #importar arquivo CSV.
colnames(dd) <- c("data", "renda") #alterar nome das colunas.

View(df) #visualizar tabela. 
View(dd) #visualizar tabela.



