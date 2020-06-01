source('covid_new.R', encoding = 'utf-8')
library(shinydashboard)

dashboard <- dashboardPage(
  dashboardHeader(title = 'Covid no Brasil',
                  dropdownMenu(type = 'messages',
                               messageItem(
                                 from = 'Criado por Leonardo Sampaio',
                                 message = 'Dataset obtido no Kaggle'
                               ))), 
  dashboardSidebar(disable = T), 
  dashboardBody(
    
    fluidRow(box(leafletOutput('mapa'), width = '100%'),
             
    ),
    fluidRow(box(plotlyOutput('plot1'), status = 'primary'),
             
             box(plotlyOutput('plot2'), status = 'danger'),
             
    ),
    fluidRow(                           
      box(plotlyOutput('plot3'), status = 'primary'),
      
      box(plotlyOutput('plot4'), status = 'danger'),
      
    ),
    
    fluidRow(
      tabBox(
        title = '',
        id = 'tabset1',
        width = '100%',
        tabPanel('Estados', barPlot1),
        tabPanel('Região', barPlot2)
      )
    )
  )
)