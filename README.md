# movie_reccommendation
movie_reccommendation
#Name:Manohar Goud
##Roll No:21X05A6706
##Branch:lV year cse(data science)
##College:Narsimha Reddy Engineering College
# project title
Movie reccomendation system
# project statement
reccomending the movies to the youtube etyc apps through machine learning
import ipywidgets as  widgets
from IPython.display import display
movie_input=widgets.Text(value='Toy Story',description='Movie Title:',disabled=False)
movie_list=widgets.Output()
def ontype(data):
  with movie_list:
    movie_list.clear_output()
    title=data['new']
    if(len(title)>5):
      display(search(title))
movie_input.observe(ontype,names='value')
display(movie_input,movie_list)
# conclusion
Movie recommendation systems are an application of machine learning that aims to predict a user’s movie preferences based on their past choices and behavior. These systems use various algorithms to suggest movies to users based on their preferences. There are two main types of recommendation systems: content-based filtering and collaborative filtering. Content-based filtering recommends movies similar to the ones the user has already watched, while collaborative filtering recommends movies based on the preferences of other users with similar tastes
