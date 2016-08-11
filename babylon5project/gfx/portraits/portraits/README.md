Heres a good tip that doesnt seem to show up in the stock game files that allows you to assign specific portraits to specific leader classes.
EXAMPLE:

leader = { #scientists, generals, admirals, governor
        add = {
            trigger = {
                gender = female
                leader_class = scientist
            }
            portraits = {
                twif5
            }
        }
        add = {
            trigger = {
                gender = male
                leader_class = scientist
            }
            portraits = {
                twim5
            }
        }       
        add = {
            trigger = {
                gender = female
                leader_class = general
            }
            portraits = {
                twif2
            }
        }  
        add = {
            trigger = {
                gender = male
                leader_class = general
            }
            portraits = {
                twim2
            }
        }  
        add = {
            trigger = {
                gender = female
                leader_class = admiral
            }
            portraits = {
                twif6
            }
        } 
        add = {
            trigger = {
                gender = male
                leader_class = admiral
            }
            portraits = {
                twim6
            }
        } 
        add = {
            trigger = {
                gender = female
                leader_class = governor
            }
            portraits = {
                twif3
            }
        } 
        add = {
            trigger = {
                gender = male
                leader_class = governor
            }
            portraits = {
                twim3
            }
        }       

    }





https://www.reddit.com/r/StellarisMods/comments/4mkaxe/help_leader_class_specific_portraits/

