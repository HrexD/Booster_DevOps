pipeline {
    agent any
    
    stages {
        stage('Préparation') {
            parallel {
                stage('Réglage des machines à café ☕') {
                    steps {
                        echo 'Machines à café en mode turbo !'
                        sh 'date'
                        sh 'echo "Café préparé à : $(date)"'
                    }
                }
                stage('Affûtage des crayons ✏️') {
                    steps {
                        echo 'Réglage de la pointe...'
                        sh 'ls -la'
                        sh 'echo "Crayons affûtés et prêts à l\'emploi !"'
                    }
                }
            }
        }
        
        stage('Build & Test') {
            parallel {
                stage('Construction 🏗️') {
                    steps {
                        echo 'Assemblage des briques du projet...'
                        sh 'echo "Démarrage du build..."'
                        sh 'pwd'
                        sh 'echo "Build terminé !"'
                    }
                }
                stage('Tests 🧪') {
                    steps {
                        echo 'Lancement des tests...'
                        sh 'echo "Initialisation des tests..."'
                        sh 'ls'
                        sh 'echo "Tests terminés, résultats disponibles."'
                    }
                }
            }
        }
        
        stage('Déploiement') {
            steps {
                echo 'Déploiement en cours...'
                sh 'echo "Déploiement lancé à : $(date)"'
                sh 'echo "Déploiement terminé !"'
                echo 'Attention, la fusée est en route ! 🚀💥'
                echo 'Ça va secouer, mais ça va bien se passer... peut-être. 😅'
            }
        }
        
        stage('Notification & Célébration') {
            steps {
                echo 'Envoi des invitations à la fête de déploiement...'
                sh 'echo "Notifications envoyées à : $(date)"'
                echo 'La fête commence maintenant ! 🎉🎈'
                echo 'Chacun apporte son bug le plus bizarre... 🐛'
            }
        }
    }
    
    post {
        success {
            steps {
                echo 'La pipeline a été exécutée avec succès ! 🚀'
                sh 'echo "Pipeline exécutée avec succès à : $(date)"'
                echo 'Mission accomplie, capitaine ! 🌟'
            }
        }
        failure {
            steps {
                echo 'Oh non, la pipeline a échoué... 🛑'
                sh 'echo "Pipeline échouée à : $(date)"'
                echo 'Il est temps d\'appeler l\'équipe des super-héros ! 🦸‍♂️🦸‍♀️'
            }
        }
        always {
            steps {
                echo 'Merci d\'avoir utilisé Jenkins, à la prochaine ! 👋'
                sh 'echo "Fin de l\'exécution à : $(date)"'
                echo 'N\'oubliez pas de nourrir le poisson rouge dans le datacenter... 🐠'
            }
        }
    }
}
