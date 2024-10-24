Team-Titans.

public class TeamBio {
    private String teamName;
    private String[] members;

    public TeamBio(String teamName, String[] members) {
        this.teamName = teamName;
        this.members = members;
    }

    public void displayBio() {
        System.out.println("Team: " + teamName);
        System.out.print("Members: ");
        for (String member : members) {
            System.out.print(member + " ");
        }
        System.out.println();
    }

    public static void main(String[] args) {
        String[] teamMembers = {"SiamTheFrog", "Aminul-Shordar"};
        TeamBio team = new TeamBio("Team-Titans", teamMembers);
        team.displayBio();
    }
}
