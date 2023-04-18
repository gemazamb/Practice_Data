
# Importar librerias ------------------------------------------------------

library(tidyverse)
library(shiny)
library(dslabs)


# Carga de datos ----------------------------------------------------------

gaspminder_df<-gapminder %>% tibble()


# UI ----------------------------------------------------------------------
ui<-fluidPage(
  sidebarLayout(
    sidebarPanel(
      numericInput(
        inputId = "selectorAnio",
        label="Seleccione un año de estudio",
        value=2010, min=2005, max=2010),
      selectInput(
        inputId = "selectorcontinents",
        label="Seleccione un continents",
        choices=gaspminder_df %>% pull(continent) %>% unique(),
        selected="Asia",
        multiple=T
        
      )
    ),
    mainPanel()
  )
)

# SERVER ------------------------------------------------------------------
server<-function(input,output){
  
}


# EJECUTION ---------------------------------------------------------------
shinyApp(ui,server)

