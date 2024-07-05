pipeline {
    agent any
    
    stages {
        stage('Préparation') {
            parallel {
                stage('Réglage des machines à café ☕') {
                    steps {
                        echo 'Machines à café en mode turbo !'
                        echo 'Attention : café chaud, idées chaudes ! ☕💡'
                    }
                }
                stage('Affûtage des crayons ✏️') {
                    steps {
                        echo 'Réglage de la pointe...'
                        echo 'N\'oubliez pas les gommes anti-fautes ! 📝✨'
                    }
                }
            }
        }
        
        stage('Build & Test') {
            parallel {
                stage('Construction 🏗️') {
                    steps {
                        echo 'Assemblage des briques du projet...'
                        echo 'Tapez 1 pour construire, 2 pour réparer... 404 not found 😄'
                    }
                }
                stage('Tests 🧪') {
                    steps {
                        echo 'Lancement des tests...'
                        echo 'À la recherche des bugs perdus...'
                        echo 'Les bugs sont de drôles de créatures, attrapez-les tous ! 🐞🦋'
                    }
                }
            }
        }
        
        stage('Déploiement') {
            steps {
                echo 'Déploiement en cours...'
                echo 'Attention, la fusée est en route ! 🚀💥'
                echo 'Ça va secouer, mais ça va bien se passer... peut-être. 😅'
            }
        }
        
        stage('Notification & Célébration') {
            steps {
                echo 'Envoi des invitations à la fête de déploiement...'
                echo 'La fête commence maintenant ! 🎉🎈'
                echo 'Chacun apporte son bug le plus bizarre... 🐛'
            }
        }
    }
    
    post {
        success {
            echo 'La pipeline a été exécutée avec succès ! 🚀'
            echo 'Mission accomplie, capitaine ! 🌟'
        }
        failure {
            echo 'Oh non, la pipeline a échoué... 🛑'
            echo 'Il est temps d\'appeler l\'équipe des super-héros ! 🦸‍♂️🦸‍♀️'
        }
        always {
            echo 'Merci d\'avoir utilisé Jenkins, à la prochaine ! 👋'
            echo 'N\'oubliez pas de nourrir le poisson rouge dans le datacenter... 🐠'
        }
    }
}
