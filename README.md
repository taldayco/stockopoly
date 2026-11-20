# stockopoly

monopoly with stocks!

Hello from Thomas
Hello from Aaron
Hello from Gomez

<<<<<<< Updated upstream



Aaron's Ideas:
Obviously, we'll need a card class, something like:
class card{
public:
card(){
   id=search_id;
}

int find_id();
??? get_png(); //don't know the return type

private:
string name;
int color; //Have it correspond to the different colors-like 1 could be red, 2 could be the blues, etc.
//if stocks are treated as a card, 0 could indicate that it's a card
int id;//Could be used with graphics. Unless we use draw commands or something at runtime, we could have a bunch of PNGs
//that we just use a BST to search for. Or we could just have seperate arrays for each color, since each color only has 2-4 cards,
//linear search won't matter
=======
Aaron's Ideas: Obviously, we'll need a card class, something like: class card{ public: card(){ id=search_id; }

int find_id(); ??? get_png(); //don't know the return type

private: string name; int color; //Have it correspond to the different colors-like 1 could be red, 2 could be the blues, etc. //if stocks are treated as a card, 0 could indicate that it's a card int id;//Could be used with graphics. Unless we use draw commands or something at runtime, we could have a bunch of PNGs //that we just use a BST to search for. Or we could just have seperate arrays for each color, since each color only has 2-4 cards, //linear search won't matter
>>>>>>> Stashed changes

};

We'd also have the hand class, no need for inheritance

<<<<<<< Updated upstream
class hand{
public:

private:
int playerNumber; //corresponds to players, 1-4 for player one, player 2, etc, unless each player object has its own declared hand
vector<card> cardsInHand; //Could also be a dynamic linked list, but I think vector allocates on heap so this would be easy

};


class player{
public:
private:
hand playerHand;

};
=======
class hand{ public:

private: int playerNumber; //corresponds to players, 1-4 for player one, player 2, etc, unless each player object has its own declared hand vector cardsInHand; //Could also be a dynamic linked list, but I think vector allocates on heap so this would be easy

};

class player{ public: private: hand playerHand;

};
>>>>>>> Stashed changes
