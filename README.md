using System;

namespace Sparta_dungeon_Text_Game_
{
    internal class Program
    {

        static void mainLobby()
        {
            Console.Clear();
            MyChar character = new MyChar(01, "Warrior", 10, 5, 100, 1500);
            MyInventory inven = new MyInventory();
            MyShop shop = new MyShop();
            Console.WriteLine(" ");
            Console.WriteLine("스파르타 마을 에 오신 여러분 환영합니다. ");
            Console.WriteLine("이곳에서 던전으로 들어가기전 활동을 할 수 있습니다. ");
            Console.WriteLine(" ");
            Console.WriteLine("1. 상태 보기");
            Console.WriteLine("2. 인벤토리");
            Console.WriteLine("3. 상점 ");
            Console.WriteLine(" ");
            Console.WriteLine("원하시는 행동을 입력해주세요. ");
            string input = Console.ReadLine();
            if (input == "1")
            {
                character.ShowMyChar();
                if (character.menu == 0)
                {
                    mainLobby();
                }
            }
            else if (input == "2")
            {
                inven.ShowInven();
                if (inven.menu == 0)
                {
                    mainLobby();
                }
                else if (input == "3")
                {
                    inven.Equip();
                    if (inven.menu == 0)
                    {
                        mainLobby();
                    }
                    else if(input == "4")
                    {
                        shop.Showshop();
                        if (shop.menu == 0)
                        {
                            mainLobby();
                        }
                    }
                }
                else
                {
                    Console.WriteLine("잘못된 선택입니다.");
                    Thread.Sleep(1000);
                    mainLobby();
                }
            }
        }

        공용 정적 공극 메인(string[] args)
        {
            메인 로비();
        }
    }

    공개수업 마이인벤토리
    {
        public List<string> Inven;
        public int menu;
        public int select;

        public void ClassicInven()
        {
            Inven = new List<string>();
            string[] weapon =
            {
                "1", "무쇠갑옷", "Defend : +5", "무쇠로 만들어져 튼튼한 갑옷입니다. ", "2", "스파르타의 창", "Attack : +7", "스파르타의 전사들이 사용했다는 전설의 창입니다.", "3", "낡은 검", "Attack : +2", "쉽게 볼 수 있는 낡은 검 입니다." };
            for (int i = 0; i < weapon.Length; i++)
            {
                Inven.Add(weapon[i]);
            }
        }

        public void ShowInven()
        {
            콘솔.클리어();
            Classic Inven();
            콘솔.WriteLine("인벤토리");
            콘솔.WriteLine("보유 중인 아이템을 관리할 수 있습니다");
            콘솔.선 쓰기(""");
            콘솔.WriteLine("{아이템 목록}");
            콘솔.WriteLine("1") 장착 관리");
            콘솔.WriteLine("0. 나가기");
            콘솔.줄 쓰기("");
            콘솔.WriteLine("원하시는 행동을 입력하시오");
            콘솔.WriteLine(">"),
            메뉴 = int구문 분석(Console).선 읽기();


            콘솔.클리어();
            Classic Inven();
            콘솔.WriteLine("인벤토리 - 장착관리");
            콘솔.WriteLine("보유 중인 아이템을 관리할 수 있습니다.");
            콘솔.WriteLine("{아이템 목록}");
            (inti = 0; i < Inven)의 경우.카운트; i += 3)
            {
                콘솔.WriteLine("\t" + Inven[i] +"\t"+ Inven[i+1] +"\t"+ Inven[i+2] + "\t");
            }

            Console.WriteLine(" ");
            Console.WriteLine("0. 나가기");
            Console.WriteLine("");
            Console.WriteLine("원하시는 행동을 입력하시오");
            Console.WriteLine(">>");
            menu = int.Parse(Console.ReadLine());
        }

        public void Equip()
        {
            Console.Clear();
            ClassicInven();
            Console.WriteLine("인벤토리 - 장착관리");
            Console.WriteLine("보유 중인 아이템을 관리할 수 있습니다.");
            Console.WriteLine("{아이템 목록}");
            Console.WriteLine("{아이템 이름}  | {장비 효과} | {장비 설명} ");
            for (int i = 0; i < Inven.Count; i += 3)
                if (select == (i / 3 + 1))
                {
                    Console.WriteLine("[E]" + "[" + (i / 3 + 1) + "]" + "\t" + Inven[i] + "\t" + "\t" + Inven[i + 1] + "\t" + "\t" + "\t" + Inven[i + 2] + "\t");
                }
                else
                {
                    Console.WriteLine("[" + (i / 3 + 1) + "]" + "\t" + "\t" + Inven[i] + "\t" + "\t" + "\t" + Inven[i + 1] + "\t" + "\t" + "\t" + Inven[i + 2] + "\t");
                }

            Console.WriteLine(" ");
            Console.WriteLine("0. 나가기");
시스템 사용;
            콘솔.WriteLine("원하시는 행동을 입력하시오");
네임스페이스 스파르타_던전_텍스트_게임_
            메뉴 = int구문 분석(Console).선 읽기();
    내부 클래스 프로그램
    }

    공개수업 마이샵()
    {
        공개 목록<string> 상점;
        공개 메뉴
        공개적으로 선택합니다.

        공용 보이드 아머 무기점()
        {
            Shop = 새 목록<string>(;
            끈[] 갑옷 =
            {
                "-1 수련자 갑옷", "Defend : +5", "수련에 도움을 주는 갑옷입니다.", "-2 무쇠갑옷", "Defend : +9", ".무쇠로 만들어져 튼튼한 갑옷입니다.",
                "-3 스파르타의 갑옷", "Defend : +15", "스파르타의 전사들이 사용했다는 전설의 갑옷입니다."
            };
            (inti = 0; i < 방어구)를 위해.길이; i++)
            {
                샵.추가(armor[i]);
            }

            string[] 무기 =
            {
                "낡은 검", "Attack : +2", "쉽게 볼 수 있는 낡은 검 입니다.", "청동 도끼", "Attack : +5", "어디선가 사용됐던거 같은 도끼 입니다.",
                "스파르타의 창", "Attack : +7", "스파르타의 전사들이 사용했다는 전설의 창 입니다."
            };
            (int j = 0; j < weapon.길이; j++)
            {
                샵.Add(weapon[j]);
            }
        }

        공공 공실 쇼샵()
        {
            콘솔.클리어();
            아머 무기 상점();
            콘솔.WriteLine("상점");
            콘솔.WriteLine("필요한 아이템을 얻을 수 있는 상점 입니다. ");
            콘솔.WriteLine("{아이템 목록}");
            콘솔.WriteLine("{아이템 이름}      | {장비 효과} | {장비 설명} ");
            (inti = 0; i < Shop.카운트; i += 3)
            {
                콘솔.줄 쓰기("\t" + Shop[i] + "\t" + "\t" + Shop[i + 1] + "\t" + Shop[i + 2] + "\t");
            }

            (int j = 0; j < Shop.카운트; j + = 3)
            {
                콘솔.줄 쓰기("\t" + 상점[j] + "\t" + 상점[j + 1] + "\t" + 상점[+2] + "\t");
            }

            콘솔.선 쓰기(""");
            콘솔.WriteLine("0. 나가기");
            콘솔.줄 쓰기("");
            콘솔.WriteLine("원하시는 행동을 입력하시오");
            콘솔.WriteLine(">"),
            메뉴 = int구문 분석(Console).선 읽기();
        }
    }
}
