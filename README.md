C#
```C#
namespace Slonie
{
    
    class Elephant
    {
        public string Name;
        public int EarSize;

        public void WhoAmI()
        {
            MessageBox.Show("Moje uszy mają " + EarSize + " centymetrów szerokości", Name + " mówi");
        }

        public void TellMe(string message, Elephant whoSaidIt)
        {
            MessageBox.Show(whoSaidIt.Name + " mówi: " + message);
        }

        public void SpeakTo(Elephant whoToTalkTo, string message)
        {
            whoToTalkTo.TellMe(message, this);
        }

    }
}

![alt text](https://github.com/Xabarex/holly-molly/blob/master/Screenshot_1.png)
