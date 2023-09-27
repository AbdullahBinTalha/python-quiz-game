# python-quiz-game
#a program using only basic level python to be easily understand by  people
# making list of all the science questions 
question_sci_list = ['Q1:what is the most abundant element in the air?',
                     'Q2:Which one is the basic unit of all living things?',
                     'Q3:Which of the smallest part of all living things in which many activities take place?',
                     'Q4:what is the most common compound found in ocean',
                     'Q5:The first scientist who discovered the cell?',
                     'Q6:How many types of cells are there?',
                     'Q7:Which is the outer part of a cell in animals?',
                     'Q8:Prokaryotic and eukaryotic are?',
                     'Q9:Cells are very tiny and only can be seen with a?',
                     'Q10:Chromosomes are present in?'
]
#making list of all the science choices
choices_sci_list = ['a:nitrogen   ''b:oxygen   ''c:carbon   ''d:calcium', #1
                   'a:Molecule   ''b:Atom   ''c:None   ''d:Call',#2
                   'a:Cell wall   '  'b:Nucleus   ' 'c:Cytoplasm   ''d:Chromosomes',#3
                    'a:H2SO4   ''b:H2O   ''c:NaCL   ''d:none',#4
                    'a:Robert hook   ''b:Crook   ''c:Dalton   ''d:Chadwick',#5
                   'a:150   ''b:200   ''c:67   ''d:100',#6
                   'a:Cell membrane   ''b:Cell wall   ''c:Nucleus   ''d:Cyctoplasm',#7
                    'a:Molecules   ''b:Cells   ''c:None of them   ''d:Atoms',#8
                   'a:Camera   ''b:Telescope   ''c:Microscope   ''d:Naked eye',#9
                    'a:Nucleus   ''b:Cell wall   ''c:Cell membrane   ''d:Cytoplasm'#10
                    ]
#making list for all correct ans of science
all_sci_correct_ans = ['Q1:a:nitrogen',
                  'Q2:b:atom',
                  'Q3:d:chromosome'
                  'Q4:b:H2O',
                  'Q5:a:Robert Hook',
                  'Q6:b:200',
                  'Q7:a:cell membrane',
                  'Q8:b:cells',
                  'Q9:c:Microscope',
                  'Q10:d:cytoplasm'
                  ]
#making list for all GK Questions
question_GK_list = ['Q1:Which bridge in Turkey connects Asia and Europe?',
                    'Q2:Buddhism is worlds fourth-largest religion. It is believed to be originated in?',
                    'Q3:Who was appointed as the first president of the All-India Muslim League?',
                    'Q4:The “Hawaii” state of the United States is located about 2000 miles from the US mainland in the?',
                    'Q5:Which countries have successfully landed a robot on the planet Mars?',
                    'Q6:What is the name of artificial intelligence company of Elon Musk launched in July 2023?',
                    'Q7:Asia is the worlds most populous continent. The second most populous continent of the world is?',
                    'Q8:The hottest month ever recorded on Earth was?',
                    'Q9:Internet uses ____ to communicate between devices and networks?',
                    'Q10:Which key combination is used to center align text?'
                    ]
#making list for all GK choices
Choices_GK_list=['a: Golden Gate Bridge     b: Akashi Kaikyo Bridge     c: Bosphorus Bridge     d: Royal Gorge Bridge',#1
                  'a: China      b: India     c: Japan      d: Thailand',#2
                   'a: Allama Iqbal      b: Sir Aga Khan     c: Mohsin-ul-Mulk     d: Muhammad Ali Johar',#3 
                   'a: Atlantic ocean      b: Pacific ocean     c: Arctic ocean      d: Mediterranean Sea',#4
                   'a: China and United States     b: Russia and United States     c: China and Russia     d:France and Germany',#5
                   'a: Meta     b: X  c: xAI  d: Giga',#6
                   'a: Africa    b: Europe     c: South America    d: North America',#7
                   'a: June 1968    b: July 1968     c: June 2023   d: July 1913',#8
                   'a: HTTPS    b: email    c: website    d: internet protocol suite',#9
                   'a: CTRL + B     b: CTRL + C     c: CTRL + E    d: CTRL + Z',#10
                      ]
# making list for all correct choices
all_GK_correctans = ['Q1:c:Bosphorus Bridge',
                    'Q2:a: China ',
                    'Q3:b:Sir Aga Khan III',
                    'Q4:b:Pacific ocean',
                    'Q5:a:China and United States',
                    'Q6:c:xAI',
                    'Q7:a:Africa',
                    'Q8:d:July 1913  ',
                    'Q9:d:internet protoocol suite ',
                    'Q10:c:CTRL + E'  ]

 # making a condition
admin = input ('are you a admin, enter yes or no:  ')
#making a login system
if admin == 'yes':
    user_input_name =(input("enter your user name :"))
    user_input_pass =(input("Enter your password:"))

    if user_input_name == 'admin' and user_input_pass == '!@#$':
        file = open('b.txt','r')
        lines = file.readlines()
        for f in (lines):
            print(f)
    else:
        print('wrong input!')

else:
    
        #asking for interested genre
        print('a:Science')
        print('b:General kowledge') 
        game = input('Select the one you are interested in: ') 
        #making a counter 
        total_score = 0
        if game == 'a': 
        #printing the science program
        ##########################################SCIENCE###############################################################################
                print('you have selected the science: ')
                print('------------MCQS--------------------')
                print('select the correct option')
                ###################1#########################
                print('----------------------------------')
                print(question_sci_list[0])
                print(choices_sci_list[0])
                l = input('enter the correct option: ') 
                if l == 'a':
                    total_score+=1 
                else:
                    print('Your Answer was wrong!')
                    ######################2#######################
                print('----------------------------------')

                print(question_sci_list[1])
                print(choices_sci_list[1])
                l = input('enter the correct option: ') 
                if l == 'b':
                    total_score+=1
                else:
                    print('Your Answer was wrong!')
                ####################3################################
                    print('----------------------------------')

                print(question_sci_list[2])
                print(choices_sci_list[2])
                l = input('enter the correct option: ') 
                if l == 'd':
                    total_score+=1
                else:
                    print('Your Answer was wrong!')
                ################4#######################
                print('----------------------------------')

                print(question_sci_list[3])
                print(choices_sci_list[3])
                l = input('enter the correct option: ') 
                if l == 'b':
                    total_score+=1
                else:
                    print('Your Answer was wrong!')
                ###############5#####################
                print('----------------------------------')

                print(question_sci_list[4])
                print(choices_sci_list[4])
                l = input('enter the correct option: ') 
                if l == 'a':
                    total_score+=1
                else:
                    print('Your Answer was wrong!')
                #################6###################
                print('----------------------------------')

                print(question_sci_list[5])
                print(choices_sci_list[5])
                l = input('enter the correct option: ') 
                if l == 'b':
                    total_score+=1
                else:
                    print('Your Answer was wrong!')
                ################7#####################
                print('----------------------------------')

                print(question_sci_list[6])
                print(choices_sci_list[6])
                l = input('enter the correct option: ') 
                if l == 'a':
                    total_score+=1 
                else:
                    print('Your Answer was wrong!')
                #################8########################
                print('----------------------------------')
            
                print(question_sci_list[7])
                print(choices_sci_list[7])
                l = input('enter the correct option: ') 
                if l == 'd':
                    total_score+=1 
                else:
                    print('Your Answer was wrong!')
                ################9####################
                print('----------------------------------')

                print(question_sci_list[8])
                print(choices_sci_list[8])
                l = input('enter the correct option: ') 
                if l == 'c':
                    total_score+=1 
                else:
                    print('Your Answer was wrong!')
                ################10#####################
                print('----------------------------------')

                print(question_sci_list[9])
                print(choices_sci_list[9])
                l = input('enter the correct option: ') 
                if l == 'd':
                    total_score+=1
                else:
                    print('Your Answer was wrong!')
                ########################################################
                print('Thank you for playing')
                print('your total score is:')
                print(total_score)
                print('--------------------------------')
                option = input('Do you wish to see all the correct answers? enter yes or no: ')
                if option == 'yes':
                    for i in (all_sci_correct_ans):
                        print(i)
                else:
                    print('ok thank you for coming')


        elif game == 'b':
                #printing all GK questions
                #################################GENERAL KNOWLEGDE########################################################3
                print('you have selected general knowledge')
                print('------------MCQS--------------------')
                print('select the correct option')
                    #######################!####################
                print(question_GK_list[0])
                print(Choices_GK_list[0])
                r = input('enter the correct option: ') 
                if r == 'c':
                    total_score+=1 
                else:
                    print('Your Answer was wrong!')
                ######################2#######################
                print('-----------------------------------')
                print(question_GK_list[1])
                print(Choices_GK_list[1])
                r = input('enter the correct option: ') 
                if r == 'a':
                    total_score+=1
                else:
                    print('Your Answer was wrong!')
                ####################3################################
                print('-----------------------------------')
                print(question_GK_list[2])
                print(Choices_GK_list[2])
                r = input('enter the correct option: ') 
                if r == 'b':
                    total_score+=1
                else:
                    print('Your Answer was wrong!')
                ################4#######################
                print('-----------------------------------')
                print(question_GK_list[3])
                print(Choices_GK_list[3])
                r = input('enter the correct option: ') 
                if r == 'b':
                    total_score+=1
                else:
                    print('Your Answer was wrong!')
                ###############5#####################
                print('-----------------------------------')
                print(question_GK_list[4])
                print(Choices_GK_list[4])
                r = input('enter the correct option: ') 
                if r == 'a':
                    total_score+=1
                else:
                    print('Your Answer was wrong!')
                #################6###################
                print('-----------------------------------')
                print(question_GK_list[5])
                print(Choices_GK_list[5])
                r = input('enter the correct option: ') 
                if r == 'c':
                    total_score+=1
                else:
                    print('Your Answer was wrong!')
                ################7#####################
                print('-----------------------------------')
                print(question_GK_list[6])
                print(Choices_GK_list[6] )
                r = input('enter the correct option: ') 
                if r == 'a':
                    total_score+=1 
                else:
                    print('Your Answer was wrong!')
                #################8########################  
                print('-----------------------------------')  
                print(question_GK_list[7])
                print(Choices_GK_list[7])
                r = input('enter the correct option: ') 
                if r == 'd':
                    total_score+=1 
                else:
                    print('Your Answer was wrong!')
                ################9####################
                print('-----------------------------------')
                print(question_GK_list[8])
                print(Choices_GK_list[8])
                r = input('enter the correct option: ') 
                if r == 'd':
                    total_score+=1 
                else:
                    print('Your Answer was wrong!')
                ################10#####################
                print('-----------------------------------')
                print(question_GK_list[9])
                print(Choices_GK_list[9])
                r = input('enter the correct option: ') 
                if r == 'c':
                    total_score+=1
                else:
                    print('Your Answer was wrong!')
                ###########################################
                print('-----------------------------------')
                print('your total score is:')
                print(total_score)
                print('-----------------------------------')
                option2 = input('Do you wish to see all the correct answers? Enter yes or no: ')
                if option2 == 'yes':
                    for i in (all_GK_correctans):
                       print(i)
                else:
                        print('ok thank you for coming')

        else:
            print('!you can only select from the given choices!')

# The admin file

Here are some questions that you can be added from each group 
--------------------SCIENCE---------------------------------------
Q1:what is the symbol of iron?
a:Na          b:I
c:Fe          c:c
------------------------------------------------------------------
Q2:what is the name of the scientists who discovered Gravity?
a:Aelbert Einstien            b:Sir Frankestien
c:Isaac Newton                d:Charles Babbbage
------------------------------------------------------------------
Q3:how many chambers of heart are there?
a:6                    b:2
c:3                    d:4
------------------------------------------------------------------
Q4:you can get vitamin C from?
a:fish               b:sunlight
c:beef               d:none
------------------------------------------------------------------
Q5:lava is an example of?
a:solid              b:plasma
c:liquid             d:gas

--------------------GENERAL KNOWLEDGE---------------------------------------
Q1:which  is national flower of Pakistan?
a:Jasmine                 b:Rose
c:sun flower              d:none 
------------------------------------------------------------------
Q2:What is the national animal of Wales?
a:Unicorn                 b:Wale
c:Dragon                  c:Megladon
------------------------------------------------------------------
Q3:one nibble is equals to?
a:4 bits               b:6 bits
c:8 bits               d:16 bits
------------------------------------------------------------------
Q4:Electric motor was invented by?
a:Sir Isaac Newton          b:Faraday
c:Rutherford                c:Henry Cevendish
------------------------------------------------------------------
Q5:Battery was invented by?
a:Alessandro Volta             b:Micheal Faraday
c:Georg ohm                    d:none
#XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX#
