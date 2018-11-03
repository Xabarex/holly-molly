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

![screenshot_1](https://user-images.githubusercontent.com/33806899/47953365-f2f6cf00-df7c-11e8-8791-e7159111c15c.png)

