horario = 0
minutero = 0
segundero = 0
def setup():
    size(700,500)
def draw():
    global horario
    global minutero
    global segundero
    background(175)
    fill(252,5,220)
    ellipse(100,horario,70,70)
    if horario > height:
        horario = 0
    else:
        horario= map(hour(),0,24,0, height)
    fill(124,199,225)
    ellipse(width / 2,minutero,70,70)
    if minutero > height:
       minutero = 0
    else:
        minutero= map(minute(),0,59,0, height)
    fill(118,225,98)
    ellipse(600,segundero,70,70)
    if segundero > height:
        segundero = 0
    else:
        segundero= map(second(),0,59,0, height)
        
