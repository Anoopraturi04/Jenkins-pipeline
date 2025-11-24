 pipeline{

    agent any

    parameters{
        // syntax to declare a variable
        string(name: 'PERSON', defaultValue: 'Anoop', description: 'Name of an Employee')
        string(name: 'Tool', defaultValue: 'Jenkins', description: 'Tool to learn')    
        choice(name: 'ENV', choices: ['Dev','Test','prod'], description: 'These are env')
        choice(name: 'branch', choices: ['dev','master','main'])

    // choice = list of values/multiple values 
    // parameterts are used/reffered in the stages   
    }  ///test

    stages{
        stage('Job1'){
            steps{
                // steps to print variable values
                // use the parameters => ${params.name}
                // go to the parameter section, go to the given parameter name and fetch the value 
                
                echo "Hello ${params.PERSON}" // Hello Anoop
                echo "Learn the DevOps tool ${params.Tool}" // Learn the DevOps tool Jenkins
                echo "Work in the Enviornment: ${params.ENV}"  
                echo "Work on the git branch: ${params.branch}"
            }
        }
    }
 }